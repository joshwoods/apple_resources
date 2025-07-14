

- Foundation
- FileWrapper
-  matchesContents(of:) 

Instance Method

# matchesContents(of:)

Indicates whether the contents of a file wrapper matches a directory, regular file, or symbolic link on disk.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func matchesContents(of url: URL) -> Bool
```

## Parameters 

`url`  

URL of the file-system node with which to compare the file wrapper.

## Return Value

true when the contents of the file wrapper match the contents of `url`, false otherwise.

## Discussion

The contents of files are not compared; matching of regular files is based on file modification dates. For a directory, children are compared against the files in the directory, recursively.

Because children of directory file wrappers are not read immediately by the init(url:options:) method unless the `NSFileWrapperReadingImmediate` reading option is used, even a newly-created directory file wrapper might not have the same contents as the directory on disk. You can use this method to determine whether the file wrapper’s contents in memory need to be updated.

If the file wrapper needs updating, use the read(from:options:) method with the `NSFileWrapperReadingImmediate` reading option.

This table describes which attributes of the file wrapper and file-system node are compared to determine whether the file wrapper matches the node on disk:

| File-wrapper type | Comparison determinants                   |
|-------------------|-------------------------------------------|
| Regular file      | Modification date and access permissions. |
| Directory         | Children (recursive).                     |
| Symbolic link     | Destination pathname.                     |

## See Also

### Related Documentation

var fileAttributes: [String : Any]

A dictionary of file attributes.

### Updating File Wrappers

func needsToBeUpdated(fromPath: String) -> Bool

Indicates whether the file wrapper needs to be updated to match a given file-system node.

Deprecated

func update(fromPath: String) -> Bool

Updates the file wrapper to match a given file-system node.

Deprecated

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

