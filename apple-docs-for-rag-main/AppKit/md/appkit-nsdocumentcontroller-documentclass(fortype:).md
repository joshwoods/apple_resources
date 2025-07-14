

- AppKit
- NSDocumentController
-  documentClass(forType:) 

Instance Method

# documentClass(forType:)

Returns the `NSDocument` subclass associated with a given document type.

macOS

``` source
@MainActor
func documentClass(forType typeName: String) -> AnyClass?
```

## Parameters 

`typeName`  

The name of a document type, specified by `CFBundleTypeName` in the application’s `Info.plist` file.

The document type must be one the receiver can read.

## Return Value

Returns the `NSDocument` subclass associated with `documentTypeName`. If the class cannot be found, returns `nil`.

## See Also

### Managing Document Types

var documentClassNames: [String]

An array of strings representing the custom document classes supported by this app.

var defaultType: String?

Returns the name of the document type that should be used when creating new documents.

func displayName(forType: String) -> String?

Returns the descriptive name for the specified document type, which is used in the File Format pop-up menu of the Save As dialog.

func typeForContents(of: URL) throws -> String

Returns, for a specified URL, the document type identifier to use when opening the document at that location, if successful.

