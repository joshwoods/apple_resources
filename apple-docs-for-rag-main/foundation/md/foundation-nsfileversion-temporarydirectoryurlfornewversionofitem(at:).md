

- Foundation
- NSFileVersion
-  temporaryDirectoryURLForNewVersionOfItem(at:) 

Type Method

# temporaryDirectoryURLForNewVersionOfItem(at:)

Creates and returns a temporary directory to use for saving the contents of the file.

macOS 10.7+

``` source
class func temporaryDirectoryURLForNewVersionOfItem(at url: URL) -> URL
```

## Parameters 

`url`  

The URL of the file whose contents you want to save.

## Return Value

A URL identifying the temporary directory in which to create a the new file. You must delete the directory specified by this URL after you have created the file and moved it to its proper location.

## Discussion

You can use this method in situations where you want to create a file in a temporary location. For example, you might use this method when saving the contents of a file to disk for the first time. When you finish creating the temporary file, move it to a more appropriate location, such as the user’s `Documents` directory. You must delete the directory returned by this method when you are done with it.

## See Also

### Getting the Version of a File

class func currentVersionOfItem(at: URL) -> NSFileVersion?

Returns the most recent version object for the file at the specified URL.

class func otherVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns all versions of the specified file except the current version.

class func version(itemAt: URL, forPersistentIdentifier: Any) -> NSFileVersion?

Returns the version of the file that has the specified persistent ID.

