

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.UserIdentity
-  JPKIPassContents.UserIdentity.AuthenticationType 

Enumeration

# JPKIPassContents.UserIdentity.AuthenticationType

Defines valid authentication types associated with the user identity.

iOS 18.0+iPadOS 18.0+

``` source
enum AuthenticationType
```

## Overview

Use of the systemBiometric authentication requires you to set the NSFaceIDUsageDescription usage description.

## Topics

### Types of authentication

case pin(String)

The PIN associated with the user identity.

case systemBiometric

Authentication using biometric information.

## See Also

### Identifying the pass user

let userIdentity: JPKIPassContents.UserIdentity?

Allows for access to the user identity, if present in the JPKI applet.

func changePIN(from: String, to: String) async throws

A function that allows for the change of the PIN associated with the user identity.

