

- Account &amp; Organizational Data Sharing
- JWKSet
-  JWKSet.Keys 

Dictionary

# JWKSet.Keys

An object that defines a single JSON Web Key.

AccountOrganizationalDataSharing 1.0+

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

The key type parameter setting. Use the value `RSA`.

`n`

`string`

The modulus value for the RSA public key.

`use`

`string`

The intended use for the public key.

## Attributes 

Possible types:

## Overview

JWK is an open standard (RFC 7517) that defines a data structure to represent cryptographic keys.

