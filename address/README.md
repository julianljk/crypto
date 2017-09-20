# Address

## Address Physical Characteristics
- 26-35 Alphanumeric characters (usually 34 characters)
- Contains random characters with the exception of uppercase O, number 0, uppercase I, lowercase l to avoid ambiguity 
- Several of the characters inside a Bitcoin address are used as a checksum so that typographical errors can be automatically found and rejecte
- Begins with 1-3 (representing possible destination)
- Can be generated at no cost for the user
- Transactions do not have a "from" address (?can this be exploited)

## Address Properties

### Addresses are a single-use token 
A user can have multiple addresses and each address is used for a transaction (?can addresses be consolidated if an address doesn't have enough btc?)

### Addresses can be created offline 
Does not require a connection to the network. Potential reasons to create address offline:

1. E-commerce websites: Pre-generate addresses for customers to use (?is the paying party assigned the address, or is that just an address that the website uses to receive payment)
2. HD Wallets?: Generates a seed token which can be used to allow untrusted systems to generate unlimited number of addresses without the ability to spend the bitcoin received. 

### Addreses are case sensitive
Avoid hand typing an address. Incorrect addresses will get rejected. The probability that a mistyped address is accepted as being valid is 1 in 232, that is, approximately 1 in 4.29 billion.

### Proving you receive with an address
If I'm trying to send bitcoin to someone, how can I verify that the address i'm sending to is the address of the guy I think I'm sending to. Fortunately, he can send me a signed message that associates itself to an address, so I know he actually owns that address (an adversary cannot mimic this without ownership of the address). 

### Multi-signature addresses
What if you wanted to have multiple people to verify a payment before it goes through. You can do so via multi-signature addresses. This has the ability of putting a trusted co-signer that can verify the legibility of a transaction (lawyers, clearing houses), while not giving them control over the funds, (only the user that initiates the transaction can decide where to spend the money).

## Misconceptions

### Address reuse 
Addresses are not intended to be used more than once. 

### Address balances 
Addresses are not accounts nor do they carry balances. They only receive funds. You cannot send from an address. 
## Address formats
1. Common P2PKH which begin with the number 1, eg: 1BvBMSEYstWetqTFn5Au4m4GFg7xJaNVN2.
2. Newer P2SH type starting with the number 3, eg: 3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy.

