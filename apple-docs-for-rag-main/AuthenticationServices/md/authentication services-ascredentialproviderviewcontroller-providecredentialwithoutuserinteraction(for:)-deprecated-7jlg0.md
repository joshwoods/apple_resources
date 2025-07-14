

- Authentication Services
- ASCredentialProviderViewController
-  provideCredentialWithoutUserInteraction(for:) Deprecated

Instance Method

# provideCredentialWithoutUserInteraction(for:)

Attempts to provide the user-requested credential with no further user interaction.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func provideCredentialWithoutUserInteraction(for credentialIdentity: ASPasswordCredentialIdentity)
```

Deprecated

Use provideCredentialWithoutUserInteraction(for:) instead.

## Parameters 

`credentialIdentity`  

The credential identity for which a credential should be provided.

## Discussion

When the user selects a credential identity from the QuickType bar, the system calls the provideCredentialWithoutUserInteraction(for:) method to ask your extension to provide the corresponding credential.

Call the context’s completeRequest(withSelectedCredential:completionHandler:) method to provide the credential if the extension can do so without further user interaction. If not—for example, because the user must first unlock a password database—call the cancelRequest(withError:) method instead using an error with domain ASExtensionErrorDomain and code userInteractionRequired. In turn, the system calls your prepareInterfaceToProvideCredential(for:) method to give your extension a chance to present an interface to handle the needed user interaction.

You can alternatively call the cancel method to indicate other error conditions using one of the codes in ASExtensionError.Code.

Note

When the system calls this method, your extension’s view controller isn’t showing. Don’t attempt to perform any user interaction from this method.

## See Also

### Deprecated methods

func prepareInterfaceToProvideCredential(for: ASPasswordCredentialIdentity)

Prepares the interface for a user interaction, like a database login, that enables it to access and return the credential for the given identity.

Deprecated

