

- Authentication Services
-  ASPasskeyAssertionCredential 

Class

# ASPasskeyAssertionCredential

A passkey assertion credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class ASPasskeyAssertionCredential
```

## Overview

Create a passkey assertion credential to provide a response to a passkey authentication challenge from your credential provider extension. Call completeAssertionRequest(using:completionHandler:), passing your passkey assertion credential.

## Topics

### Creating a passkey assertion credential

init(userHandle: Data, relyingParty: String, signature: Data, clientDataHash: Data, authenticatorData: Data, credentialID: Data)

Initializes a passkey assertion credential object.

### Accessing credential information

var authenticatorData: Data

The authenticator data of the application that created this passkey assertion credential.

var clientDataHash: Data

A hash of the client data for this credential.

var credentialID: Data

The identifier for this credential.

var relyingParty: String

The relying party associated with this passkey.

var signature: Data

The cryptographic signature of this credential.

var userHandle: Data

The user handle of this passkey.

### Initializers

convenience init(userHandle: Data, relyingParty: String, signature: Data, clientDataHash: Data, authenticatorData: Data, credentialID: Data, extensionOutput: ASPasskeyAssertionCredentialExtensionOutput?)

### Instance Properties

var extensionOutput: ASPasskeyAssertionCredentialExtensionOutput?

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationCredential
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Providing credentials

func completeRequest(withSelectedCredential: ASPasswordCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected credential.

func completeAssertionRequest(using: ASPasskeyAssertionCredential, completionHandler: ((Bool) -> Void)?)

Complete the passkey assertion request by providing the user-selected passkey credential.

func completeRegistrationRequest(using: ASPasskeyRegistrationCredential, completionHandler: ((Bool) -> Void)?)

Complete the registration request by providing the newly-created passkey credential.

func completeOneTimeCodeRequest(using: ASOneTimeCodeCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected one-time passcode (OTP).

class ASPasswordCredential

A password credential.

class ASPasskeyRegistrationCredential

A passkey registration credential.

class ASOneTimeCodeCredential

A one-time passcode (OTP) credential.

