

- AppKit
- NSDocument
-  writableTypes 

Type Property

# writableTypes

Returns the types of data the receiver can write natively and any types filterable to that native type.

macOS

``` source
@MainActor
class var writableTypes: [String] { get }
```

## Return Value

An array of `NSString` objects representing the writable document types.

## See Also

### Managing File Type Information

class var readableTypes: [String]

Returns the types of data the receiver can read natively and any types filterable to that native type.

class func isNativeType(String) -> Bool

Returns a Boolean value that indicates whether the document can read and write the data natively.

func writableTypes(for: NSDocument.SaveOperationType) -> [String]

Returns the names of the types to which this document can be saved for a specified kind of save operation.

func fileNameExtension(forType: String, saveOperation: NSDocument.SaveOperationType) -> String?

Returns a filename extension that can be appended to a base filename, for a specified file type and kind of save operation.

