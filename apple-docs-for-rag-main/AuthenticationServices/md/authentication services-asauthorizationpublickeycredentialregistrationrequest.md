

- Authentication Services
-  ASAuthorizationPublicKeyCredentialRegistrationRequest 

Protocol

# ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
protocol ASAuthorizationPublicKeyCredentialRegistrationRequest : NSCopying, NSSecureCoding, NSObjectProtocol
```

## Topics

### Getting the properties

var attestationPreference: ASAuthorizationPublicKeyCredentialAttestationKind

The type of attestation you’re requesting.

**Required**

var challenge: Data

Arbitrary data that the client signs as proof of a valid registration or attestation.

**Required**

var displayName: String?

A user-visible name for the credential, such as the account’s user name.

**Required**

var name: String

A user-visible name that identifies a credential.

**Required**

var relyingPartyIdentifier: String

The domain name of the website for the credential.

**Required**

var userID: Data

Data that the relying party associates with the credential.

**Required**

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

A preference for whether the authenticator attempts to verify the user at the time of sign-in.

**Required**

## Relationships

### Inherits From

- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

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

class ASPasskeyCredentialRequest

A class that represents a request to supply a passkey credential.

class ASPasskeyCredentialRequestParameters

A class that represents information about a passkey credential request.

