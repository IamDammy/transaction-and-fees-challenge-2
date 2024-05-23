# transaction-and-fees-challenge-2

# SOLANA CALCULATOR
A simple smart contract that implements an on chain calculator.

# Description
This smart contract calculator is to demonstrait how to write a native Solana Program with the methodolgy of seperating the code in the following way, entrypoing, instructions, state, process. The entrypoint is the starting point of the program and passes the instructions and data to the processor. The processor communicates with the instructions module where the instruction and data is deserialized and then passes that data back to the processor where the processor determines which instruction to invoke. Then the processor will communicate with the state module and deserilize any account data, then the processor will update the state data and the data is serialized once again and stored.

The Calculator itself impelemnts all basic arithimtic opperations. The general usage is to first load a operand into the outpout account with a set instruction then followed by an instruction that is either an ADD, SUB, MUL, DIV, or MOD operation with an opperand passed as data that will be applied to the output account. This implementation allows for chaining multiple mathmatical opperations with series of instructions for each opperation.

# Example 
SET 5 ADD 5 SUB 2
 the expected result will be 8

 # Getting Started

 # Installing

 #### run a local test validator with the below code to get you connected with the local net

 solana-test-validator 

 #### Generate a new wallet with the following code
 solana-keygen new

 #### Airdrop sol to your wallet with the following code
 solana airdrop 1
 Note you can only airdrop 1 sol at a time so u can continue to airdrop into your account as many times as u want 

#### Deploy the smart contract or the program to the local devnet with the following code
solana program deploy /home/guild-audits/solana_calculator/program/target/deploy/solana_calculator.so

#### check to see if your programme as been deployed successfully
solana program show 1Ys6e3jVXdzmJYrvLQYpNe9v6nKCspFgddxQvZSYsKw
Note: solana program show programId

# Operator
* SET: setting the initial operator
* ADD: the **ADDITION** operator
* SUB: the operator for **SUBTRACTION**
* MUL: the operator for **MULTIPLICATION**
* DIV: the operator for **DIVISION**
* MOD: the operator for **MODULO** operations

Generally, the command is operator + operand + operator + operand  and so on.....

# Authors
Ajayi Damola Ramon
@justtA7J

# License
This project is licensed under the MIT License - see the LICENSE.md file for details






