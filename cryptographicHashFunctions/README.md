# Cryptographic Hash Function 
## Properties
- Special class of hash function.
- Map <Data<String>, String<?128bits?>>, data is variable length, string is fixed length.
- One way function (not feasible to invert).

## Implications:
- Only way to retrieve the data is via brute force
    or 
- Rainbow table of matched hashes

## Desirable characteristics
- Deterministic
- Fast to hash
- Only way of attaining plain text is via brute force
- No correlation between distance of cipertext and distance of plaintext ("edit distance")
- 1:1 hash mapping

## Metrics of security
- Pre-image resistance

    Given a hash value h it should be difficult to find any message m such that h = hash(m). This concept is related to that of one-way function. Functions that lack this property are vulnerable to preimage attacks.

- Second pre-image resistance

    Given an input m1 it should be difficult to find different input m2 such that hash(m1) = hash(m2). Functions that lack this property are vulnerable to second-preimage attacks.

- Collision resistance

    It should be difficult to find two different messages m1 and m2 such that hash(m1) = hash(m2). Such a pair is called a cryptographic hash collision. This property is sometimes referred to as strong collision resistance. It requires a hash value at least twice as long as that required for preimage-resistance; otherwise collisions may be found by a birthday attack.

    - Colision resistance implies second pre-image resistance but the converse is not true
    - Attacker cannot modify input, m1,  data without changing the value of hash(m1).

- Second pre-image resistance vs Collision resistance
    - Second pre-image resistance prevents an attacker from crafting a document with the same hash as a document the attacker cannot control
    - Collision resistance prevents an attacker from creating two distinct documents with the same hash.       

## Examples
- MD5 
- SHA-0 
- SHA-1 
- SHA-2
- SHA-3