

- AppKit
- NSPasteboard
-  write(\_:) 

Instance Method

# write(\_:)

Writes the serialized contents of the specified file wrapper to the pasteboard.

macOS

``` source
func write(_ wrapper: FileWrapper) -> Bool
```

## Parameters 

`wrapper`  

The file wrapper to write to the pasteboard.

## Return Value

true if the data was successfully written, otherwise false.

## Discussion

Writes the serialized contents of the file wrapper `wrapper` to the receiver and declares the data to be of type `NSFileContentsPboardType` and also of a type appropriate for the file’s extension (as returned by the `NSCreateFileContentsPboardType` function when passed the files extension), if it has one. If `wrapper` does not have a preferred filename, this method raises an exception.

## See Also

### Writing Data (macOS 10.5 and Earlier)

func declareTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

func addTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Adds promises for the specified types to the first pasteboard item.

func writeFileContents(String) -> Bool

Writes the contents of the specified file to the pasteboard.

