

- Foundation
- NSData
-  write(to:atomically:) 

Instance Method

# write(to:atomically:)

Writes the data object’s bytes to the location specified by a given URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    to url: URL,
    atomically: Bool
) -> Bool
```

## Parameters 

`url`  

The location to which to write the receiver’s bytes. Only `file://` URLs are supported.

`atomically`  

If true, the data is written to a backup location, and then—assuming no errors occur—the backup location is renamed to the name specified by `aURL`; otherwise, the data is written directly to `aURL`. `atomically` is ignored if `aURL` is not of a type the supports atomic writes.

## Return Value

true if the operation succeeds, otherwise false.

## Discussion

Since at present only `file://` URLs are supported, there is no difference between this method and write(toFile:atomically:), except for the type of the first argument.

This method may not be appropriate when writing to publicly accessible files. To securely write data to a public location, use FileHandle instead. For more information, see Securing File Operations in Secure Coding Guide.

## See Also

### Writing Data to a File

func write(toFile: String, atomically: Bool) -> Bool

Writes the data object’s bytes to the file specified by a given path.

func write(toFile: String, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the file specified by a given path.

func write(to: URL, options: NSData.WritingOptions) throws

Writes the data object’s bytes to the location specified by a given URL.

struct WritingOptions

Options for methods used to write data objects.

