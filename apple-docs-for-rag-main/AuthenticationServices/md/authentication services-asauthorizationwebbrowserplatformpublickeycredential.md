

- Authentication Services
-  ASAuthorizationWebBrowserPlatformPublicKeyCredential 

Structure

# ASAuthorizationWebBrowserPlatformPublicKeyCredential

A structure that describes a passkey stored in the keychain, or managed by a third-party credential manager.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
struct ASAuthorizationWebBrowserPlatformPublicKeyCredential
```

## Overview

Use ASAuthorizationWebBrowserPlatformPublicKeyCredential to describe passkeys in your browser app’s user interface so the person can choose a passkey. Get the chosen passkey’s credentialID to create a ASAuthorizationPlatformPublicKeyCredentialDescriptor that identifies the passkey to the operating system.

## Topics

### Describing credentials

let customTitle: String

A string the person can supply to describe this credential.

let name: String

The user name for the account associated with this credential.

let providerName: String

The name of the app that manages this credential, or “iCloud Keychain” if it’s the operating system.

let relyingParty: String

The relying party that issues challenges for this credential.

let userHandle: Data

A unique identifier for the user account at the relying party.

### Identifying credentials

let credentialID: Data

The identifier the operating system uses for this credential.

## Relationships

### Conforms To

- Sendable

## See Also

### Using passkeys

func platformCredentials(forRelyingParty: String) async -> [ASAuthorizationWebBrowserPlatformPublicKeyCredential]

Gets a list of passkeys available for authenticating with the given relying party.

