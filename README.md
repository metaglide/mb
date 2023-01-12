##
Project for motoko bootcamp

## check balance 

```
dfx wallet --network ic balance

```

## create empty canister in in network with 1 trillion cycles,
## build wasm module 
## deploy wasm module to the empty cansiter

```

dfx canister --network ic create mb --with-cycles 1000000000000

dfx build --network ic mb

dfx canister --network ic install mb

```

## check for the installation by calling greet function

```

dfx canister --network ic call mb greet '(" world")'

```
