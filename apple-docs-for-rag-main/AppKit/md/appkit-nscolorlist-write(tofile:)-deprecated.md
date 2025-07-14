

- AppKit
- NSColorList
-  write(toFile:) Deprecated

Instance Method

# write(toFile:)

Saves the color list to the file at the specified path.

macOS 10.0–10.14Deprecated

``` source
func write(toFile path: String?) -> Bool
```

Deprecated

Use write(to:) instead.

## Parameters 

`path`  

The path at which to save the color list. If `path` is a directory, the receiver is saved in a file named listname`.clr` in that directory (where listname is the name with which the receiver was initialized).

If `path` includes a filename, this method saves the file under that name. If `path` is `nil`, the file is saved as listname`.clr` in the user’s private colorlists directory.

## Return Value

true upon success and false if the method fails to write the file.

## See Also

### Writing and Removing Color List Files

func write(to: URL?) throws

Saves the color list to the file at the specified URL.

func removeFile()

Removes the file from which the list was created, if the file is in a standard search path and owned by the user.

