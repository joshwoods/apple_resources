

- Authentication Services
- ASCredentialProviderViewController
-  prepareInterfaceToProvideCredential(for:) Deprecated

Instance Method

# prepareInterfaceToProvideCredential(for:)

Prepares the interface for a user interaction, like a database login, that enables it to access and return the credential for the given identity.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func prepareInterfaceToProvideCredential(for credentialIdentity: ASPasswordCredentialIdentity)
```

Deprecated

Use prepareInterfaceToProvideCredential(for:) instead.

## Parameters 

`credentialIdentity`  

The credential identity for which a credential should be provided.

## Discussion

The system calls this method when your extension can’t provide the requested credential without user interaction. Set up the view controller for any user interaction required to provide the requested credential. Limit user interaction to operations required for providing the requested credential, like showing an authentication UI to unlock the user’s passwords database.

Call the context’s completeRequest(withSelectedCredential:completionHandler:) to provide the credential. Alternatively, if an error occurs, call cancelRequest(withError:) instead and pass an error with domain ASExtensionErrorDomain and an appropriate error code from ASExtensionError.Code. For example, if your app can’t find the credential identity in the database, pass an error with code ASExtensionError.Code.credentialIdentityNotFound.

## See Also

### Deprecated methods

func provideCredentialWithoutUserInteraction(for: ASPasswordCredentialIdentity)

Attempts to provide the user-requested credential with no further user interaction.

Deprecated

