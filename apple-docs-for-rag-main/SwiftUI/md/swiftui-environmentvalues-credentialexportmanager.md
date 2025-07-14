

- SwiftUI
- EnvironmentValues
-  credentialExportManager 

Instance Property

# credentialExportManager

This environment variable is for SwiftUI clients of the credential exchange API. An example usage might look like:

AuthenticationServicesSwiftUIiOS 18.2+iPadOS 18.2+macOS 15.2+visionOS 2.2+

``` source
var credentialExportManager: ASCredentialExportManager { get }
```

## Discussion

```
struct CredentialExchangeManagerExample: View {
    @Environment(\.credentialExchangeManager) private var credentialExchangeManager

    var body: some View {
        Button("Export Credentials") {
            Task {
                do {
                    let credentialData = getCredentialData() // defined elsewhere
                    try await credentialExchangeManager.exportCredentials(credentialData)
                } catch {
                    // code to handle the export error
                }
            }
        }
    }
}
```

