

- AppKit
- NSDocument
-  readableTypes 

Type Property

# readableTypes

Returns the types of data the receiver can read natively and any types filterable to that native type.

macOS

``` source
@MainActor
class var readableTypes: [String] { get }
```

## Return Value

An array of `NSString` objects representing the readable document types.

## See Also

### Related Documentation

class func canConcurrentlyReadDocuments(ofType: String) -> Bool

Returns a Boolean value that indicates whether the receiver reads multiple documents of the given type concurrently.

### Managing File Type Information

class var writableTypes: [String]

Returns the types of data the receiver can write natively and any types filterable to that native type.

class func isNativeType(String) -> Bool

Returns a Boolean value that indicates whether the document can read and write the data natively.

func writableTypes(for: NSDocument.SaveOperationType) -> [String]

Returns the names of the types to which this document can be saved for a specified kind of save operation.

func fileNameExtension(forType: String, saveOperation: NSDocument.SaveOperationType) -> String?

Returns a filename extension that can be appended to a base filename, for a specified file type and kind of save operation.

