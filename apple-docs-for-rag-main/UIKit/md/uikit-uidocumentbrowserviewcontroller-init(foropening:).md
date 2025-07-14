

- UIKit
- UIDocumentBrowserViewController
-  init(forOpening:) 

Initializer

# init(forOpening:)

Initializes and returns a document browser view controller that can open the specified file types.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
init(forOpening contentTypes: [UTType]?)
```

## Parameters 

`contentTypes`  

An array of uniform type identifiers. If `nil`, the browser uses the document types that the CFBundleDocumentTypes key specifies in the app’s `Info.plist` file.

For detailed instructions about setting the `CFBundleDocumentTypes` key, see Setting up a document browser app.

For more information about type identifiers, see Uniform Type Identifiers.

## See Also

### Creating a document browser

Adding a document browser to your app

Give users access to their local or remote documents from within your app.

