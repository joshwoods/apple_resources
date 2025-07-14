

- AppKit
- NSPasteboard
-  readFileWrapper() 

Instance Method

# readFileWrapper()

Reads data representing a file’s contents from the receiver and returns it as a file wrapper.

macOS

``` source
func readFileWrapper() -> FileWrapper?
```

## Return Value

A file wrapper containing the pasteboard data, or `nil` if the receiver contained no data of type `NSFileContentsPboardType`.

## Discussion

In macOS 10.5 and earlier, the file contents pboard type allowed you to synthesize a pboard type for a file’s contents based on the file’s extension. In macOS 10.5 and later, using the UTI of a file to represent its contents now replaces this functionality.

## See Also

### Reading Data (macOS 10.5 and Earlier)

func readFileContentsType(NSPasteboard.PasteboardType?, toFile: String) -> String?

Reads data representing a file’s contents from the receiver and writes it to the specified file.

