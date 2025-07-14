

- Authentication Services
- ASCredentialProviderViewController
-  prepareCredentialList(for:requestParameters:) 

Instance Method

# prepareCredentialList(for:requestParameters:)

Prepares the interface to display a list of passkey and password credentials from which the user can select.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func prepareCredentialList(
    for serviceIdentifiers: [ASCredentialServiceIdentifier],
    requestParameters: ASPasskeyCredentialRequestParameters
)
```

## Parameters 

`serviceIdentifiers`  

An array of service identifiers that provide a hint about the service for which the user needs credentials.

`requestParameters`  

Information about the passkey request.

## Discussion

The system calls this method to tell your extension’s view controller to prepare to present a list of credentials, when there’s an active passkey request in the app or website. After calling this method, the system presents the view controller to the user.

Use the given `serviceIdentifiers` array to filter or prioritize the credentials to display. The service identifier array might be empty, but your extension should still show credentials from which the user can pick.

Items in the array with lower indices represent more specific identifiers for which a credential’s requested. For example, if the array contains identifiers `[m.example.com, example.com]`, the item `m.example.com` represents the more specific service that requires a credential.

If the person selects a passkey credential, use the `requestParameters` object to complete the request using the selected credential.

## See Also

### Selecting a credential

func prepareCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of credentials from which the user can select.

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

class ASPasskeyCredentialRequestParameters

A class that represents information about a passkey credential request.

