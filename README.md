# Running a Relayer

## Setup

This relayer requires Rust and solana development environment.

Refer jito instruction.

    https://jito-foundation.gitbook.io/mev/jito-relayer/running-a-relayer until Section "RPC Server" for setup instructions.

--> Create a new folder (e.g. "explorer-relayer") and add your      validator-node authentication files: 
    public.pem, private.pem, keypair.json

## Download project

Run this command to download explorer relayer.

      git clone https://github.com/Explorer/relayer.git

      cd relayer

      cargo build

## Run

-------------------------------------------------------- Run directly in your relayer folder(recommend for non-familar) -----------------------------------------------

You can run the relayer directly in the relayer folder.

follow this instruction.

 cd relayer
 cargo run -- --keypair-path ../explorer-relayer/keypair.json \
          --signing-key-pem-path ../explorer-relayer/private.pem \
          --verifying-key-pem-path ../explorer-relayer/public.pem