

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.Certificate 

Structure

# JPKIPassContents.Certificate

The certificate data associated with an identity document.

iOS 18.0+iPadOS 18.0+

``` source
struct Certificate where IdentityType : JPKIPassContents.Identity
```

## Overview

Use this structure to access the underlying certificate data you use to sign the pass.

## Topics

### Defining data

let data: Data

The result of the signed data from the requested digital identity in X.509 DER format.

## See Also

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

struct SigningIdentity

The authentication for signing user identification.

struct Signature

The resulting signed data and certificate you use to sign the pass.

struct AuthenticationRequest

The user authentification request based on the generics type.

protocol Identity

Defines the common functionality that JPKI digital identities support.

