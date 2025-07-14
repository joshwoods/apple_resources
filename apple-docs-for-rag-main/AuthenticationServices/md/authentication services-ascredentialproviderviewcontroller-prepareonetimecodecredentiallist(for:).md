

- Authentication Services
- ASCredentialProviderViewController
-  prepareOneTimeCodeCredentialList(for:) 

Instance Method

# prepareOneTimeCodeCredentialList(for:)

Prepares the interface to display a list of one-time passcodes (OTPs) that people can select from.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func prepareOneTimeCodeCredentialList(for serviceIdentifiers: [ASCredentialServiceIdentifier])
```

## Parameters 

`serviceIdentifiers`  

An array of service identifiers that provide a hint about the service that people need an OTP for.

## Mentioned in 

Providing one-time passcodes to AutoFill

## Overview

## Discussion

The system calls this method to tell your extension’s view controller to prepare a list of OTPs to present. After calling this method, the system presents the view controller to the person.

Use the given `serviceIdentifiers` array to filter or prioritize the credentials to display. The service identifier array might be empty, but your extension still shows credentials that the person can select from.

Items in the array with lower indices represent more specific identifiers for which an OTP’s requested. For example, if the array contains identifiers `[m.example.com, example.com]`, the item `m.example.com` represents the more specific service that requires an OTP.

When someone selects an OTP displayed by your view controller, represent the passcode as an ASOneTimeCodeCredential and pass it to the system by calling completeOneTimeCodeRequest(using:completionHandler:):

```
let credential = ASOneTimeCodeCredential(code: otpCode)
await extensionContext.completeOneTimeCodeRequest(using: credential)
```

Always provide a way for someone to cancel the operation from your view controller, for example, by including a Cancel button in the navigation bar. When someone cancels the operation, call cancelRequest(withError:), using the error domain ASExtensionErrorDomain and code userCanceled:

```
let error = NSError(domain: ASExtensionErrorDomain,
                    code: ASExtensionError.userCanceled.rawValue)
extensionContext.cancelRequest(withError: error)
```

The system dismisses your view controller after you call either the completion or cancellation method.

## See Also

### Selecting a credential

func prepareCredentialList(for: [ASCredentialServiceIdentifier])

Prepares the interface to display a list of credentials from which the user can select.

func prepareCredentialList(for: [ASCredentialServiceIdentifier], requestParameters: ASPasskeyCredentialRequestParameters)

Prepares the interface to display a list of passkey and password credentials from which the user can select.

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

