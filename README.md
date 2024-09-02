# JWT-JSON-Web-Token-
This is the repository contains complete documentation on JWT.


## What is JWT (JSON Web Token) ?
-> JSON Web Token (JWT) is a compact, URL-safe means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object, which is then digitally signed or encrypted using a secret key or a public/private key pair.

---


## How is JWT structured ?
-> A JWT consists of three parts, separated by dots (.):

1. Header: Contains metadata about the type of token (JWT) and the signing algorithm being used (e.g., HMAC, RSA).

2. Payload: Contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims:
  i. Registered Claims: Predefined claims that are optional but recommended (e.g., iss for issuer, exp for expiration time).
  ii. Public Claims: Custom claims that can be defined by those using JWTs but must avoid collisions with registered claims.
  iii. Private Claims: Custom claims that are unique to the issuer and the consumer.
3. Signature: Used to verify the token's integrity and ensure that the sender of the JWT is who it says it is. It is created by taking the encoded header, the encoded payload, a secret, and the algorithm specified in the header, and then signing that.

### Example of JWT :
```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c

```