

- Authentication Services
- ASCredentialProviderViewController
-  prepareInterface(forPasskeyRegistration:) 

Instance Method

# prepareInterface(forPasskeyRegistration:)

Prepare the view controller to show user interface for registering a new passkey.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func prepareInterface(forPasskeyRegistration registrationRequest: any ASCredentialRequest)
```

## Parameters 

`registrationRequest`  

The passkey registration request.

## Discussion

The system calls this method when the user selects your extension to create a passkey. Your app and extension must declare the key ProvidesPasskeys with value `YES` in the ASCredentialProviderExtensionCapabilities dictionaries of their information property lists to be available for the user to select. The system presents your extension’s authentication user interface before creating the passkey.

Call the context’s completeRegistrationRequest(using:completionHandler:) method with the created passkey credential. Alternatively, if an error occurs, call cancelRequest(withError:), using ASExtensionErrorDomain as the error domain and an appropriate error code from ASExtensionError.Code.

## See Also

### Selecting a credential

func prepareCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of credentials from which the user can select.

func prepareCredentialList(for: [ASCredentialServiceIdentifier], requestParameters: ASPasskeyCredentialRequestParameters)

Prepares the interface to display a list of passkey and password credentials from which the user can select.

func prepareOneTimeCodeCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of one-time passcodes (OTPs) that people can select from.

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

