

- AppKit
- NSDocument
-  isNativeType(\_:) 

Type Method

# isNativeType(\_:)

Returns a Boolean value that indicates whether the document can read and write the data natively.

macOS

``` source
@MainActor
class func isNativeType(_ type: String) -> Bool
```

## Parameters 

`type`  

The string that identifies the document type to test.

## Return Value

true if the document type is a native type; otherwise, false.

## See Also

### Managing File Type Information

class var readableTypes: [String]

Returns the types of data the receiver can read natively and any types filterable to that native type.

class var writableTypes: [String]

Returns the types of data the receiver can write natively and any types filterable to that native type.

func writableTypes(for: NSDocument.SaveOperationType) -> [String]

Returns the names of the types to which this document can be saved for a specified kind of save operation.

func fileNameExtension(forType: String, saveOperation: NSDocument.SaveOperationType) -> String?

Returns a filename extension that can be appended to a base filename, for a specified file type and kind of save operation.

