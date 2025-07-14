

- AppKit
- NSPasteboard
-  readFileContentsType(\_:toFile:) 

Instance Method

# readFileContentsType(\_:toFile:)

Reads data representing a file’s contents from the receiver and writes it to the specified file.

macOS

``` source
func readFileContentsType(
    _ type: NSPasteboard.PasteboardType?,
    toFile filename: String
) -> String?
```

## Parameters 

`type`  

The pasteboard data type to read. You should generally specify a value for this parameter. If you specify `nil`, the filename extension (in combination with the `NSCreateFileContentsPboardType` function) is used to determine the type.

`filename`  

The file to receive the pasteboard data.

## Return Value

The name of the file into which the data was actually written.

## Discussion

Data of any file contents type should only be read using this method. If data matching the specified type is not found on the pasteboard, data of type `NSFileContentsPboardType` is requested.

macOS 10.6 and later

In macOS 10.5 and earlier, the file contents pboard type allowed you to synthesize a pboard type for a file’s contents based on the file’s extension. In macOS 10.5 and later, using the UTI of a file to represent its contents now replaces this functionality.

### Special Considerations

You must send an availableType(from:) or types message before invoking readFileContentsType(_:toFile:).

## See Also

### Related Documentation

func writeFileContents(String) -> Bool

Writes the contents of the specified file to the pasteboard.

### Reading Data (macOS 10.5 and Earlier)

func readFileWrapper() -> FileWrapper?

Reads data representing a file’s contents from the receiver and returns it as a file wrapper.

