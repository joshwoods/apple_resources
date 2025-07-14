

- Authentication Services
- ASCredentialProviderViewController
-  prepareInterfaceForExtensionConfiguration() 

Instance Method

# prepareInterfaceForExtensionConfiguration()

Prepares the interface to enable the user to configure the extension.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
func prepareInterfaceForExtensionConfiguration()
```

## Discussion

The system calls this method after the user enables your extension in Settings. Use this method to prepare a user interface for configuring the extension. You can also use the method to tell the system what credential identities your extension supports by adding them to the shared ASCredentialIdentityStore instance. Any identities you add become available as AutoFill suggestions.

After finishing configuration, tell the system to dismiss your view controller by calling the context’s completeExtensionConfigurationRequest() method.

Note

To receive a call to this method, specify the ShowsConfigurationUI key with a value of `YES` in the ASCredentialProviderExtensionCapabilities dictionary, within the NSExtensionAttributes dictionary in the extension’s Information Property List.

## See Also

### Configuring the credential provider extension

class ASCredentialIdentityStore

A container that your extension fills to provide credentials through the QuickType bar.

