

- Authentication Services
- ASCredentialProviderViewController
-  provideCredentialWithoutUserInteraction(for:) 

Instance Method

# provideCredentialWithoutUserInteraction(for:)

Attempts to provide the user-requested credential with no further user interaction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func provideCredentialWithoutUserInteraction(for credentialRequest: any ASCredentialRequest)
```

## Parameters 

`credentialRequest`  

The credential request.

## Mentioned in 

Providing one-time passcodes to AutoFill

## Discussion

After the person selects a credential identity, the system creates a credential request. The contents of the request depend on the type of credential requested. If the person requests a password or one-time passcode (OTP), the credential request (a ASPasswordCredentialRequest or ASOneTimeCodeCredentialRequest) contains a credential identity. If the person requests a passkey, the ASPasskeyCredentialRequest also contains information about the passkey assertion challenge.

The system calls provideCredentialWithoutUserInteraction(for:) to enhance the user experience. If your credential provider extension can provide the credential without user interaction, call the relevant completion method on the extension context. For password credential requests, call completeRequest(withSelectedCredential:completionHandler:). For passkey credential requests, call completeAssertionRequest(using:completionHandler:). For OTP requests, call completeOneTimeCodeRequest(using:completionHandler:).

If your extension requires user interaction to provide the credential, like when someone needs to unlock their credentials database, call cancelRequest(withError:). Use the error domain ASExtensionErrorDomain, and the code ASExtensionError.Code.userInteractionRequired.

If an error occurs, call cancelRequest(withError:) using the error domain ASExtensionErrorDomain and an appropriate code from ASExtensionError.Code.

As your view controller isn’t presented while the system calls this method, don’t show or use any user interface from this method.

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

