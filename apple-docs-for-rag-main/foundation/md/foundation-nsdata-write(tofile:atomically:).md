

- Foundation
- NSData
-  write(toFile:atomically:) 

Instance Method

# write(toFile:atomically:)

Writes the data object’s bytes to the file specified by a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    toFile path: String,
    atomically useAuxiliaryFile: Bool
) -> Bool
```

## Parameters 

`path`  

The location to which to write the receiver’s bytes. If `path` contains a tilde (~) character, you must expand it with expandingTildeInPath before invoking this method.

`useAuxiliaryFile`  

If true, the data is written to a backup file, and then—assuming no errors occur—the backup file is renamed to the name specified by `path`; otherwise, the data is written directly to `path`.

## Return Value

true if the operation succeeds, otherwise false.

## Discussion

This method may not be appropriate when writing to publicly accessible files. To securely write data to a public location, use FileHandle instead. For more information, see Securing File Operations in Secure Coding Guide.

## See Also

### Writing Data to a File

func write(toFile: String, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the file specified by a given path.

func write(to: URL, atomically: Bool) -> Bool

Writes the data object’s bytes to the location specified by a given URL.

func write(to: URL, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the location specified by a given URL.

struct WritingOptions

Options for methods used to write data objects.

