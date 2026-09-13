# Midnight Counter
> A simple smart contract on Midnight to increment a counter using private witness disclosure.

## Contract Address
| Network  | Address                          |
|----------|----------------------------------|
| Preview  | [PLACEHOLDER]                    |
| Preprod  | [PLACEHOLDER]                    |

## What This Does
This contract demonstrates how to maintain a public counter on the Midnight ledger. Users can increment this counter, but they must provide a private witness (the amount to add). This private amount is then explicitly disclosed to the network to be added to the public state.

## Privacy Model
- What is PUBLIC (on-chain, visible to anyone): The current value of the `counter` state variable.
- What is PRIVATE (private witness, never on-chain): The initial `amount_to_add` provided by the user.
- What the user PROVES without revealing: The user proves they know an amount to add, which they then disclose deliberately to update the counter.

## Tech Stack
- Midnight network, Compact language, Node.js v22, Docker

## Prerequisites
- Node.js v22
- Docker (for running the proof server)
- Compact compiler

## Setup
1. Clone the repository: `git clone https://github.com/Dhanshree-atre/NewMoon1.git`
2. Run the proof server: `docker run -d -p 6300:6300 midnightnetwork/proof-server`
3. Compile the contract: `compact compile`

## Run Tests
`npm test`

## Initial Idea
[LEAVE PLACEHOLDER — I will fill this in manually]

## Screenshots
[LEAVE PLACEHOLDER — I will add compile output and contract address screenshots]
