

- Authentication Services
-  ASPasskeyRegistrationCredential 

Class

# ASPasskeyRegistrationCredential

A passkey registration credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class ASPasskeyRegistrationCredential
```

## Overview

Create a passkey registration credential to provide a response to a passkey registration request from your credential provider extension. Call completeRegistrationRequest(using:completionHandler:), passing your passkey registration credential.

## Topics

### Creating a passkey registration credential

init(relyingParty: String, clientDataHash: Data, credentialID: Data, attestationObject: Data)

Initializes a passkey registration credential object.

### Accessing credential information

var attestationObject: Data

The attestation object for this passkey.

var clientDataHash: Data

A hash of the client data for this credential.

var credentialID: Data

The identifier for this credential.

var relyingParty: String

The relying party associated with this passkey.

### Initializers

convenience init(relyingParty: String, clientDataHash: Data, credentialID: Data, attestationObject: Data, extensionOutput: ASPasskeyRegistrationCredentialExtensionOutput?)

### Instance Properties

var extensionOutput: ASPasskeyRegistrationCredentialExtensionOutput?

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

class ASPasskeyAssertionCredential

A passkey assertion credential.

class ASOneTimeCodeCredential

A one-time passcode (OTP) credential.

