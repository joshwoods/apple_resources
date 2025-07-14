

- Sign in with Apple REST API
- JWKSet
-  JWKSet.Keys 

Object

# JWKSet.Keys

An object that defines a single JSON Web Key.

Sign in with Apple REST API 1.0+

``` source
object JWKSet.Keys
```

## Properties

`alg`

`string`

The encryption algorithm used to encrypt the token.

`e`

`string`

The exponent value for the RSA public key.

`kid`

`string`

A 10-character identifier key, obtained from your developer account.

`kty`

`string`

The key type parameter setting. You must set to “RSA”.

`n`

`string`

The modulus value for the RSA public key.

`use`

`string`

The intended use for the public key.

