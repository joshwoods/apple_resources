

- Foundation
- FileWrapper
-  needsToBeUpdated(fromPath:) Deprecated

Instance Method

# needsToBeUpdated(fromPath:)

Indicates whether the file wrapper needs to be updated to match a given file-system node.

macOS 10.0–10.10Deprecated

``` source
func needsToBeUpdated(fromPath path: String) -> Bool
```

Deprecated

Use matchesContents(of:) instead.

## Parameters 

`path`  

File-System node with which to compare the file wrapper.

## Return Value

false when the file wrapper needs to be updated to match `node`, false otherwise.

## Discussion

This table describes which attributes of the file wrapper and `node` are compared to determine whether the file wrapper needs to be updated:

| File-wrapper type | Comparison determinants                   |
|-------------------|-------------------------------------------|
| Regular file      | Modification date and access permissions. |
| Directory         | Member hierarchy (recursive).             |
| Symbolic link     | Destination pathname.                     |

### Special Considerations

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of matchesContents(of:).

## See Also

### Related Documentation

var fileAttributes: [String : Any]

A dictionary of file attributes.

### Updating File Wrappers

func matchesContents(of: URL) -> Bool

Indicates whether the contents of a file wrapper matches a directory, regular file, or symbolic link on disk.

func update(fromPath: String) -> Bool

Updates the file wrapper to match a given file-system node.

Deprecated

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

