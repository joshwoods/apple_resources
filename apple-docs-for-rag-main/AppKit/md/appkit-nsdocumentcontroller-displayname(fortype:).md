

- AppKit
- NSDocumentController
-  displayName(forType:) 

Instance Method

# displayName(forType:)

Returns the descriptive name for the specified document type, which is used in the File Format pop-up menu of the Save As dialog.

macOS

``` source
@MainActor
func displayName(forType typeName: String) -> String?
```

## Parameters 

`typeName`  

The name of a document type, specified by `CFBundleTypeName` in the application’s `Info.plist` file.

## Return Value

The descriptive name for the document type specified by `documentTypeName`. If there is no descriptive name, returns `documentTypeName`.

## Discussion

For a document-based application, supported document types are specified in the `Info.plist` file by the `CFBundleDocumentTypes` array. Each document type is specified by a dictionary in this array, and is named by the `CFBundleTypeName` attribute. You can provide a descriptive, localized, representation of this name by providing a corresponding entry in the `InfoPlist.strings` file(s). For example, given an `Info.plist` file that contains the following fragment:

```

    CFBundleDocumentTypes

            CFBundleTypeName
            BinaryFile
            CFBundleTypeExtensions

                binary

```

you could provide a descriptive name by adding an entry in the `InfoPlist.strings` file:

```
BinaryFile = "Binary file format";
```

## See Also

### Managing Document Types

var documentClassNames: [String]

An array of strings representing the custom document classes supported by this app.

var defaultType: String?

Returns the name of the document type that should be used when creating new documents.

func documentClass(forType: String) -> AnyClass?

Returns the `NSDocument` subclass associated with a given document type.

func typeForContents(of: URL) throws -> String

Returns, for a specified URL, the document type identifier to use when opening the document at that location, if successful.

