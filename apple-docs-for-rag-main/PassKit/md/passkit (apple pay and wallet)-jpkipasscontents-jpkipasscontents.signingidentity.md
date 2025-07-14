

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.SigningIdentity 

Structure

# JPKIPassContents.SigningIdentity

The authentication for signing user identification.

iOS 18.0+iPadOS 18.0+

``` source
struct SigningIdentity
```

## Overview

Use this structure to define valid signature identity authentication.

## Topics

### Signing identity authentication

let signingIdentity: JPKIPassContents.SigningIdentity?

Allows access to the signing identity, if present in the JPKI applet.

func changePassword(from: String, to: String) async throws

A function that allows you to change the password associated with the signing identity.

enum AuthenticationType

Defines the valid user authentication request options for the signing identity.

## Relationships

### Conforms To

- JPKIPassContents.Identity

## See Also

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

struct Signature

The resulting signed data and certificate you use to sign the pass.

struct Certificate

The certificate data associated with an identity document.

struct AuthenticationRequest

The user authentification request based on the generics type.

protocol Identity

Defines the common functionality that JPKI digital identities support.

