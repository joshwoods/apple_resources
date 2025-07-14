

- Authentication Services
- ASCredentialProviderViewController
-  prepareCredentialList(for:) 

Instance Method

# prepareCredentialList(for:)

Prepares the interface to display a list of credentials from which the user can select.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
func prepareCredentialList(for serviceIdentifiers: [ASCredentialServiceIdentifier])
```

## Parameters 

`serviceIdentifiers`  

An array of service identifiers that provide a hint about the service for which the user needs credentials.

## Discussion

The system calls this method to tell your extension’s view controller to prepare to present a list of credentials. After calling this method, the system presents the view controller to the user.

Use the given `serviceIdentifiers` array to filter or prioritize the credentials to display. The service identifier array might be empty, but your extension should still show credentials from which the user can pick.

Items in the array with lower indices represent more specific identifiers for which a credential’s requested. For example, if the array contains identifiers `[m.example.com, example.com]`, the item `m.example.com` represents the more specific service that requires a credential.

When the user selects a credential displayed by your view controller, encapsulate the corresponding user and password strings in an ASPasswordCredential instance and pass it to the extension context’s completeRequest(withSelectedCredential:completionHandler:) method:

```
let passwordCredential = ASPasswordCredential(user: user, password: password)
extensionContext.completeRequest(withSelectedCredential: passwordCredential)
```

Alternatively, if the user cancels the operation, call the cancelRequest(withError:) method instead with an error that indicates user cancelation:

```
let error = NSError(domain: ASExtensionErrorDomain,
                    code: ASExtensionError.userCanceled.rawValue)
extensionContext.cancelRequest(withError: error)
```

Always provide a way for the user to cancel the operation from your view controller, for example by including a cancel button in the navigation bar.

The system dismisses your view controller automatically after you call either the completion or cancelation method.

## See Also

### Selecting a credential

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

class ASPasskeyCredentialRequestParameters

A class that represents information about a passkey credential request.

