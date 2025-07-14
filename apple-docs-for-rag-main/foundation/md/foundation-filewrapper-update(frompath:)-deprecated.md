

- Foundation
- FileWrapper
-  update(fromPath:) Deprecated

Instance Method

# update(fromPath:)

Updates the file wrapper to match a given file-system node.

macOS 10.0–10.10Deprecated

``` source
func update(fromPath path: String) -> Bool
```

Deprecated

Use read(from:options:) instead.

## Return Value

true if the update is carried out, false if it isn’t needed.

## Discussion

For a directory file wrapper, the contained file wrappers are also sent update(fromPath:) messages. If nodes in the corresponding directory on the file system have been added or removed, corresponding file wrappers are released or created as needed.

### Special Considerations

Beginning with OS X v10.6, the preferred method of referring to files is with a `file://` URL. Therefore, this method has been deprecated in favor of read(from:options:).

## See Also

### Related Documentation

func updateAttachments(fromPath: String)

Updates all attachments based on files contained in the RTFD file package at the specified file path.

### Updating File Wrappers

func needsToBeUpdated(fromPath: String) -> Bool

Indicates whether the file wrapper needs to be updated to match a given file-system node.

Deprecated

func matchesContents(of: URL) -> Bool

Indicates whether the contents of a file wrapper matches a directory, regular file, or symbolic link on disk.

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

