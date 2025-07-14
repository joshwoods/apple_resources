

- Authentication Services
- ASCredentialProviderViewController
-  prepareInterfaceToProvideCredential(for:) 

Instance Method

# prepareInterfaceToProvideCredential(for:)

Prepare the view controller to show user interface for providing the requested credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func prepareInterfaceToProvideCredential(for credentialRequest: any ASCredentialRequest)
```

## Parameters 

`credentialRequest`  

The credential request.

## Mentioned in 

Providing one-time passcodes to AutoFill

## Discussion

The system calls this method when your extension can’t supply the requested credential without user interaction. Limit user interaction to operations required for providing the requested credential, like showing an authentication UI to unlock the person’s passwords database.

Call the appropriate completion method on the extension context to provide the credential. For password credentials, call completeRequest(withSelectedCredential:completionHandler:). For passkey credentials, call completeAssertionRequest(using:completionHandler:). For one-time passcodes, call completeOneTimeCodeRequest(using:completionHandler:).

Alternatively, if an error occurs, call cancelRequest(withError:) instead and pass an error with domain ASExtensionErrorDomain and an appropriate error code from ASExtensionError.Code. For example, if your app can’t find the credential identity in the database, pass an error with code ASExtensionError.Code.credentialIdentityNotFound.

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

