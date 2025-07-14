

- Authentication Services
-  ASPasskeyCredentialRequestParameters 

Class

# ASPasskeyCredentialRequestParameters

A class that represents information about a passkey credential request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class ASPasskeyCredentialRequestParameters
```

## Overview

The system creates instances of this class to handle active passkey requests, and passes them to your extension by calling prepareCredentialList(for:requestParameters:). Use the properties of the given request parameters object, along with the passkey credential that the person chooses, to construct a passkey credential response that you return to the system using completeAssertionRequest(using:completionHandler:).

## Topics

### Viewing credential request parameters

var allowedCredentials: [Data]

A list of passkey credentials that the relying party accepts for this challenge.

var clientDataHash: Data

The client data that you sign as part of the response.

var relyingPartyIdentifier: String

The relying party that issues the challenge.

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s preference for user verification.

### Instance Properties

var extensionInput: ASPasskeyAssertionCredentialExtensionInput?

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
- Sendable

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

class ASCredentialServiceIdentifier

An identifier representing a particular service for which the user needs a credential, like a web site.

protocol ASCredentialRequest

A protocol that describes a request from the user for your extension to provide a credential.

class ASPasswordCredentialRequest

A class that represents a request to supply a password credential.

class ASOneTimeCodeCredentialRequest

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASPasskeyCredentialRequest

A class that represents a request to supply a passkey credential.

