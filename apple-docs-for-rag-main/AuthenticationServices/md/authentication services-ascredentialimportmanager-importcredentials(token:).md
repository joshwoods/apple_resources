

- Authentication Services
- ASCredentialImportManager
-  importCredentials(token:) 

Instance Method

# importCredentials(token:)

Begins the credential import process.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
func importCredentials(token: UUID) async throws -> ASExportedCredentialData
```

## Parameters 

`token`  

The UUID token that the system provided in the NSUserActivity when launching the app.

## Return Value

The credential data exported from the source app.

## Discussion

When a person chooses your app to receive credentials exported from another app, the system launches your app using an NSUserActivity of type `ASCredentialExchangeActivityType`. Handle this in your app delegate for AppKit/UIKit or the onContinueUserActivity(_:perform:) modifier for SwiftUI. The `NSUserActivity` you receive contains a single UUID object in its `userInfo` field with the key `ASCredentialImportToken`; pass this UUID as the `token` parameter to this method.

This method throws an error if the import can’t proceed, which happens if the token doesn’t match what the system expects, indicating an app other than the one the export was meant for.

## See Also

### Importing credentials

struct ASExportedCredentialData

A container for credential data that your app provides to an exporter or receives from an importer.

