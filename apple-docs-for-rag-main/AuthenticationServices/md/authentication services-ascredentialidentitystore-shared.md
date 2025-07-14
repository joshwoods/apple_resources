

- Authentication Services
- ASCredentialIdentityStore
-  shared 

Type Property

# shared

The shared credential identity store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class var shared: ASCredentialIdentityStore { get }
```

## Discussion

Use the shared identity store to tell Password AutoFill about the identities for which your extension can supply credentials.

The identity store doesn’t contain passwords, but still contains sensitive information like usernames. To maintain good security, a credential provider app and its extension have a dedicated shared store that’s separate from any other app’s shared store. Further, the system doesn’t include the shared store in a device backup so the data never leaves the device. Also, the system clears the shared store if the user disables the extension in Settings.

