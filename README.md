# rust-programming

# Solana development
## Programs
### Native programs
  + System Program: for creating accounts, transferring SOL
  + Stateking Program + Voting program
### SPL (Solana program library)
  + Token program: Solana's Ethereum ERC-20 equivalent
  => interact token (include NFTs)
  
  
# How to get started.
https://learn.figment.io/tutorials/solana-101

https://github.com/figment-networks/learn-web3-dapp#-get-started


# Step to do sol
## Setup project
  + solana cli
  + DataHub key
  + keypair (for 
## Connect to solana (dev, test...)

## Create account
Solana transactions = accounts' operations

## Fund the acc with SOL
Request airdrop (solana/web3.js)

## Check balance
+ getBalance(publicKey);

## Transfer
+ Instruction: SystemProgram.transfer(from, to, amount)
+ singers[{publicKey:key, secretKey}]
+ Transaction: new Transaction().add(instructions);
+ sendAndConfirmTransaction(connection, transaction, signers) [https://solana-labs.github.io/solana-web3.js/modules.html#sendAndConfirmTransaction]

## Smart contract
+ Rust code => *compile* => program => *deploy* => smart contract
+ Pre-condition
  - Solana CLI (solana config set --url ...)
  - deploy account
    + solana-keygen new --outfile path file/key.json
    + solana config set --keypair path to file
  <p>=> Tricks (cargo-build-bpf) </p>
    + Windows: set path for Home = C:\Users\<user>
    + Run as admin
  
