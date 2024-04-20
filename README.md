If you need to install rust make sure any cargo binaries are on the path
for example 
```
export PATH="/Users/<name>/.cargo/bin:$PATH" 
```

### install solana cli
```
sh -c "$(curl -sSfL https://release.solana.com/v1.18.4/install)"
```

add it to the path, e.g.
```
export PATH="/Users/<name>/.local/share/solana/install/active_release/bin:$PATH" 
```
### make a new key with passphrase and save passphrase in password manager
```
solana-keygen new
```

### transfer some sol to the address
```
solana address
```

### confirm the transfer
```
solana balance
```

### install solana token cli
```
cargo install spl-token-cli
```

### create a token
```
spl-token create-token
```

### create account for token
This will create an account on the block chain that will hold the token
```
spl-token create-account <TOKEN ADDRESS>
```
This costs like $0.50 to make

### mint coins

Standard for 100 million
```
spl-token mint <TOKEN ADDRESS> < int amount >
```

### send coins
```
spl-token transfer --fund-recipient --allow-unfunded-recipient <TOKEN_MINT_ADDRESS> <TOKEN_AMOUNT> <RECIPIENT_WALLET_ADDRESS>
```

### Prevent minting
```
?
```

### Image
png and make it square
name it logo.png
size needs to be less than 200kb

###
```
```

###
```
```

###
```
```