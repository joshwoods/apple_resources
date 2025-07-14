

- PassKit (Apple Pay and Wallet)
-  JPKIPassContents 

Structure

# JPKIPassContents

A set of actions for viewing and updating PINs, passwords, and signing abilities associated with digital identities on the JPKI applet.

iOS 18.0+iPadOS 18.0+

``` source
struct JPKIPassContents
```

## Overview

Supports access to installed digital identities associated with the pass. You can use these actions to perform all operations to view, modify, and act on the credientials the applet contains.

## Topics

### Initializing the digital identity

init(PKPass) async throws

Initializes with the digital identity state of the provided pass.

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

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

### Error cases

enum Error

Defines a set of possible errors.

### Instance Properties

let signingIdentity: JPKIPassContents.SigningIdentity?

Allows access to the signing identity, if present in the JPKI applet.

let userIdentity: JPKIPassContents.UserIdentity?

Allows for access to the user identity, if present in the JPKI applet.

## See Also

### Japan passes

class PKAddIdentityDocumentConfiguration

Configuration to define the identity document.

class PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

