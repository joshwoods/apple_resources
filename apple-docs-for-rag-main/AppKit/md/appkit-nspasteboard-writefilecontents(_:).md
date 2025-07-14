

- AppKit
- NSPasteboard
-  writeFileContents(\_:) 

Instance Method

# writeFileContents(\_:)

Writes the contents of the specified file to the pasteboard.

macOS

``` source
func writeFileContents(_ filename: String) -> Bool
```

## Parameters 

`filename`  

The name of the file to write to the pasteboard.

## Return Value

true if the data was successfully written, otherwise false.

## Discussion

Writes the contents of the file `filename` to the receiver and declares the data to be of type `NSFileContentsPboardType` and also of a type appropriate for the file’s extension (as returned by the `NSCreateFileContentsPboardType` function when passed the files extension), if it has one.

## See Also

### Related Documentation

func readFileContentsType(NSPasteboard.PasteboardType?, toFile: String) -> String?

Reads data representing a file’s contents from the receiver and writes it to the specified file.

### Writing Data (macOS 10.5 and Earlier)

func declareTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

func addTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Adds promises for the specified types to the first pasteboard item.

func write(FileWrapper) -> Bool

Writes the serialized contents of the specified file wrapper to the pasteboard.

