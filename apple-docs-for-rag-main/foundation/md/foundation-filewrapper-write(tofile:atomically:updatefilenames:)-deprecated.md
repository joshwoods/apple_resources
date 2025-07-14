

- Foundation
- FileWrapper
-  write(toFile:atomically:updateFilenames:) Deprecated

Instance Method

# write(toFile:atomically:updateFilenames:)

Writes a file wrapper’s contents to a given file-system node.

macOS 10.0–10.10Deprecated

``` source
func write(
    toFile path: String,
    atomically atomicFlag: Bool,
    updateFilenames updateFilenamesFlag: Bool
) -> Bool
```

Deprecated

Use write(to:options:originalContentsURL:) instead.

## Parameters 

`path`  

Pathname of the file-system node to which the receiver’s contents are written.

`atomicFlag`  

true to write the file safely so that:

- An existing file is not overwritten

- The method fails if the file cannot be written in its entirety

false to overwrite an existing file and ignore incomplete writes.

`updateFilenamesFlag`  

true to update the receiver’s filenames (its filename and—for directory file wrappers—the filenames of its sub–file wrappers) be changed to the filenames of the corresponding nodes in the file system, after a successful write operation. Use this in Save or Save As operations.

false to specify that the receiver’s filenames not be updated. Use this in Save To operations.

## Return Value

true when the write operation is successful, false otherwise.

## Discussion

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of write(to:options:originalContentsURL:).

## See Also

### Related Documentation

var filename: String?

The filename of the file wrapper object

### Writing Files

func write(to: URL, options: FileWrapper.WritingOptions, originalContentsURL: URL?) throws

Recursively writes the entire contents of a file wrapper to a given file-system URL.

