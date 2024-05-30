## Local Dependencies Spec

```
rustc --version
>> rustc 1.76.0 (07dca489a 2024-02-04)

solana --version 
>> solana-cli 1.18.14 (src:d8e08244; feat:4215500110, client:SolanaLabs)

anchor --version 
>> anchor-cli 0.30.0
```

## Run Test Locally

1. Run a local validator separately
```
solana-test-validator
```

2. Run the anchor test suite without asking anchor to start the test-ledger within the project root. 
```
anchor test --skip-local-validator
```

## Error Troubleshoot Reference
1. Use solana program 1.18.5
https://solana.stackexchange.com/questions/13210/default-program-wont-build-on-anchor-0-30-ahash-0-84-no-longer-builds

2. Install BSD tar for solana-test-validator
https://solana.stackexchange.com/questions/4499/blockstore-error-when-starting-solana-test-validator-on-macos-13-0-1/4761#4761

3. Run Anchor Test by skipping local validator
https://solana.stackexchange.com/questions/5596/error-trying-to-run-anchor-test
