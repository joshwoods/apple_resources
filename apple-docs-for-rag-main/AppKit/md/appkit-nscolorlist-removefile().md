

- AppKit
- NSColorList
-  removeFile() 

Instance Method

# removeFile()

Removes the file from which the list was created, if the file is in a standard search path and owned by the user.

macOS

``` source
func removeFile()
```

## Discussion

In addition to removing the file, this method removes the color list from the contents of the availableColorLists property. If there are no outstanding references to the color list, this method might also deallocate the object.

## See Also

### Writing and Removing Color List Files

func write(to: URL?) throws

Saves the color list to the file at the specified URL.

func write(toFile: String?) -> Bool

Saves the color list to the file at the specified path.

Deprecated

