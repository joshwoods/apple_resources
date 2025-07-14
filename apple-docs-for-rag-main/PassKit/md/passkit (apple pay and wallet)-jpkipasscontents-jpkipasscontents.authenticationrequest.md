

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.AuthenticationRequest 

Structure

# JPKIPassContents.AuthenticationRequest

The user authentification request based on the generics type.

iOS 18.0+iPadOS 18.0+

``` source
struct AuthenticationRequest where IdentityType : JPKIPassContents.Identity
```

## Overview

Use this structure to define valid user authentication request options for `UserIdentity` or `SigningIdentity`.

## Topics

### Creating authentication request options

init(type: JPKIPassContents.UserIdentity.AuthenticationType)

Initializes the user authentication request options for the user identity type.

init(type: JPKIPassContents.SigningIdentity.AuthenticationType)

Initializes the user authentication request options for the signing identity type.

## See Also

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

struct SigningIdentity

The authentication for signing user identification.

struct Signature

The resulting signed data and certificate you use to sign the pass.

struct Certificate

The certificate data associated with an identity document.

protocol Identity

Defines the common functionality that JPKI digital identities support.

