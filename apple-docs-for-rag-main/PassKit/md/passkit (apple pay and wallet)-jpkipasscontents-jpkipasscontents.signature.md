

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.Signature 

Structure

# JPKIPassContents.Signature

The resulting signed data and certificate you use to sign the pass.

iOS 18.0+iPadOS 18.0+

``` source
struct Signature where IdentityType : JPKIPassContents.Identity
```

## Overview

Use this structure to access the signature associated with digital identities.

## Topics

### Defining the certificate and signed data

let certificate: JPKIPassContents.Certificate&lt;IdentityType>

The certificate associated with an identity document.

let signatureData: Data

The result of signing the data provided by the caller using the requested digital identity.

## See Also

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

struct SigningIdentity

The authentication for signing user identification.

struct Certificate

The certificate data associated with an identity document.

struct AuthenticationRequest

The user authentification request based on the generics type.

protocol Identity

Defines the common functionality that JPKI digital identities support.

