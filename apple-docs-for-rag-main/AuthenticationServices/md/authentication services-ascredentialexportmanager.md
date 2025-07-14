

- Authentication Services
-  ASCredentialExportManager 

Class

# ASCredentialExportManager

A class to manage exporting credentials.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
class ASCredentialExportManager
```

## Overview

`ASCredentialExportManager` allows your app to exchange authentication credentials like passwords and passkeys with other apps. Participating apps such as password managers can receive your exported credentials by using the ASCredentialImportManager class.

### Configure your app

To participate in credential exchange, edit your credential provider extension’s Info.plist and add the following key with a Boolean value of `YES`:

`NSExtension > NSExtensionAttributes > ASCredentialProviderExtensionCapabilities > SupportsCredentialExchange`

For iOS 18.2, visionOS 2.2, and macOS 15.2, you also need to explicitly enable credential exchange, like this:

- In iOS or visionOS, open the Settings app and enable the Settings \> Developer \> Credential Exchange switch.

- In macOS, enter the following command in Terminal:

`defaults write com.apple.AuthenticationServices.Developer CredentialExchangeEnabled -bool YES`

### Export credentials

To export credentials, your app’s interface needs to allow the person using it to select the credentials they want to export. To begin the process, call the exportCredentials(_:) method on an instance of this class. Calling this method brings up an out-of-process system UI that guides the person through the export procedure. The system UI explains the risks of exporting credentials, and then allows them to choose an app to export to. The operating system acts as an intermediary to establish the identities of the password manager apps involved and performs the exchange; this process doesn’t write any data to the file system.

When a person chooses an importer app, the system launches it, sending the NSUserActivity `ASCredentialExchangeActivity`. The importing app responds to the launch activity by calling the ASCredentialImportManager method importCredentials(token:) to receive the exported credentials.

The following example shows how to perform an export from a SwiftUI view.

```
struct CredentialExportManagerExample: View {
    @Environment(\.credentialExportManager) private var credentialExportManager

    var body: some View {
        Button("Export Credentials") {
            Task {
                do {
                    let credentialData = getCredentialData() // defined elsewhere
                    try await credentialExportManager.exportCredentials(credentialData)
                } catch {
                    // Handle the export error.
                }
            }
        }
    }
}
```

For a corresponding import code example, see ASCredentialImportManager.

## Topics

### Creating an export manager

typealias ASPresentationAnchor

A platform-specific type that indicates the kind of user interface element to use as a presentation anchor.

### Exporting credentials

func exportCredentials(ASExportedCredentialData) async throws

Begins the credential export process.

struct ASExportedCredentialData

A container for credential data that your app provides to an exporter or receives from an importer.

### Initializers

convenience init(presentationAnchor: ASPresentationAnchor)

convenience init(presentationAnchor: ASPresentationAnchor)

## See Also

### Credential migration

class ASCredentialImportManager

A class to manage importing credentials.

