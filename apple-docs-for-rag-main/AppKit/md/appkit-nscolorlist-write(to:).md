

- AppKit
- NSColorList
-  write(to:) 

Instance Method

# write(to:)

Saves the color list to the file at the specified URL.

macOS 10.11+

``` source
func write(to url: URL?) throws
```

## Parameters 

`url`  

The URL at which to store the color list. The URL must specify either a directory or file in the file system. Specify `nil` to save the color list to the user’s `~/Library/Colors` directory.

## Discussion

If `url` represents a directory, this method saves the color list in that directory in a file with the name `.clr`, where is the value of the name property. If `url` represents a file, this method saves the color list using the name you provided.

## See Also

### Writing and Removing Color List Files

func removeFile()

Removes the file from which the list was created, if the file is in a standard search path and owned by the user.

func write(toFile: String?) -> Bool

Saves the color list to the file at the specified path.

Deprecated

