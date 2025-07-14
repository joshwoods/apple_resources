

- Foundation
- NSFileVersion
-  currentVersionOfItem(at:) 

Type Method

# currentVersionOfItem(at:)

Returns the most recent version object for the file at the specified URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func currentVersionOfItem(at url: URL) -> NSFileVersion?
```

## Parameters 

`url`  

The URL of the file whose version object you want.

## Return Value

The version object representing the current version of the file or `nil` if there is no such file.

## See Also

### Getting the Version of a File

class func otherVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns all versions of the specified file except the current version.

class func version(itemAt: URL, forPersistentIdentifier: Any) -> NSFileVersion?

Returns the version of the file that has the specified persistent ID.

class func temporaryDirectoryURLForNewVersionOfItem(at: URL) -> URL

Creates and returns a temporary directory to use for saving the contents of the file.

