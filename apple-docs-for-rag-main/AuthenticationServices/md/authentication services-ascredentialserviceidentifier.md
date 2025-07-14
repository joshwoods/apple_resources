

- Authentication Services
-  ASCredentialServiceIdentifier 

Class

# ASCredentialServiceIdentifier

An identifier representing a particular service for which the user needs a credential, like a web site.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class ASCredentialServiceIdentifier
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Topics

### Creating a credential service identifier

init(identifier: String, type: ASCredentialServiceIdentifier.IdentifierType)

Initializes a credential service identifier instance.

### Identifying the credential service

var identifier: String

A string that names the identified service.

var type: ASCredentialServiceIdentifier.IdentifierType

The kind of services that the identifier represents.

enum IdentifierType

Possible values for the service identifier type.

## Relationships

### Inherits From

- NSObject

### Conforms To

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

### Selecting a credential

func prepareCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of credentials from which the user can select.

func prepareCredentialList(for: [ASCredentialServiceIdentifier], requestParameters: ASPasskeyCredentialRequestParameters)

Prepares the interface to display a list of passkey and password credentials from which the user can select.

func prepareOneTimeCodeCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of one-time passcodes (OTPs) that people can select from.

func prepareInterface(forPasskeyRegistration: any ASCredentialRequest)

Prepare the view controller to show user interface for registering a new passkey.

func prepareInterfaceToProvideCredential(for: any ASCredentialRequest)

Prepare the view controller to show user interface for providing the requested credential.

func provideCredentialWithoutUserInteraction(for: any ASCredentialRequest)

Attempts to provide the user-requested credential with no further user interaction.

func performWithoutUserInteractionIfPossible(passkeyRegistration: ASPasskeyCredentialRequest)

Perform a conditional passkey registration, if possible.

protocol ASCredentialRequest

A protocol that describes a request from the user for your extension to provide a credential.

class ASPasswordCredentialRequest

A class that represents a request to supply a password credential.

class ASOneTimeCodeCredentialRequest

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASPasskeyCredentialRequest

A class that represents a request to supply a passkey credential.

class ASPasskeyCredentialRequestParameters

A class that represents information about a passkey credential request.

