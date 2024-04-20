If you need to install rust make sure any cargo binaries are on the path
for example 
```
export PATH="/Users/kyle/.cargo/bin:$PATH" 
```

### install solana cli
```
sh -c "$(curl -sSfL https://release.solana.com/v1.18.4/install)"
```

add it to the path, e.g.
```
export PATH="/Users/kyle/.local/share/solana/install/active_release/bin:$PATH" 
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
png and make it score

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


For example:

Creating token 78ixoaksTFdFRoNoCMA3UzPWGYKa3S4uRfVeLsB11wHr under program TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA

Address:  78ixoaksTFdFRoNoCMA3UzPWGYKa3S4uRfVeLsB11wHr
Decimals:  9

Signature: 3Xe485T943qfVYK5LMH86Gy1J7Q7rU44wiFWrDFZtJMqBHCqxF1kGgWnDjQQYciVHy9FhwCiEKejgS74sU3UdGoi

spl-token create-account 78ixoaksTFdFRoNoCMA3UzPWGYKa3S4uRfVeLsB11wHr
Creating account C6VbKe4AnqfJyX5L8jtBF4sBJTWesFqKXDyLsgP8UUuy

Signature: 4SxBBu6bvAfUV2as4jwThNhoa4UCMkcya9eWE5zQ4PES6Upe2bVP69cEwLcKFg8W42CeYdLh3gsS8RGGUtbT6X9K

kyle@kyle felix-coin % spl-token mint 78ixoaksTFdFRoNoCMA3UzPWGYKa3S4uRfVeLsB11wHr 100000000
Minting 100000000 tokens
  Token: 78ixoaksTFdFRoNoCMA3UzPWGYKa3S4uRfVeLsB11wHr
  Recipient: C6VbKe4AnqfJyX5L8jtBF4sBJTWesFqKXDyLsgP8UUuy

Signature: 3SkjtXnqEFYzznARJ2vx6jVFpgHQz2tgajBjvaooosfnFWpC37eaTFSZTmZLEykJcksZb3opDHu7wSRdXQqsnxnj
