

- Foundation
- NSFileVersion
-  version(itemAt:forPersistentIdentifier:) 

Type Method

# version(itemAt:forPersistentIdentifier:)

Returns the version of the file that has the specified persistent ID.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func version(
    itemAt url: URL,
    forPersistentIdentifier persistentIdentifier: Any
) -> NSFileVersion?
```

## Parameters 

`url`  

The URL of the file whose version you want.

`persistentIdentifier`  

The persistent ID of the `NSFileVersion` object you want.

## Return Value

The file version object with the specified ID or `nil` if no such version object exists.

## See Also

### Related Documentation

var persistentIdentifier: any NSCoding

The identifier for this version of the file.

### Getting the Version of a File

class func currentVersionOfItem(at: URL) -> NSFileVersion?

Returns the most recent version object for the file at the specified URL.

class func otherVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns all versions of the specified file except the current version.

class func temporaryDirectoryURLForNewVersionOfItem(at: URL) -> URL

Creates and returns a temporary directory to use for saving the contents of the file.

