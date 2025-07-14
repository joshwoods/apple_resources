

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.UserIdentity 

Structure

# JPKIPassContents.UserIdentity

The functionality for the type of user identification.

iOS 18.0+iPadOS 18.0+

``` source
struct UserIdentity
```

## Overview

A type of digital identity that the applet can store.

## Topics

### Identifying the pass user

let userIdentity: JPKIPassContents.UserIdentity?

Allows for access to the user identity, if present in the JPKI applet.

func changePIN(from: String, to: String) async throws

A function that allows for the change of the PIN associated with the user identity.

enum AuthenticationType

Defines valid authentication types associated with the user identity.

### Instance Properties

var authenticationTriesRemaining: Int

The tries remaining before the underlying credential locks itself

## Relationships

### Conforms To

- JPKIPassContents.Identity

## See Also

### Defining access to the identity passes

struct SigningIdentity

The authentication for signing user identification.

struct Signature

The resulting signed data and certificate you use to sign the pass.

struct Certificate

The certificate data associated with an identity document.

struct AuthenticationRequest

The user authentification request based on the generics type.

protocol Identity

Defines the common functionality that JPKI digital identities support.

