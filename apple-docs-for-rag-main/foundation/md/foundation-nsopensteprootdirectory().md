

- Foundation
-  NSOpenStepRootDirectory() 

Function

# NSOpenStepRootDirectory()

Returns the root directory of the user’s system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSOpenStepRootDirectory() -> String
```

## Return Value

A string identifying the root directory of the user’s system.

## Discussion

For more information on file system utilities, see Low-Level File Management Programming Topics.

## See Also

### Related Documentation

func NSHomeDirectory() -> String

Returns the path to either the user’s or application’s home directory, depending on the platform.

func NSHomeDirectoryForUser(String?) -> String?

Returns the path to a given user’s home directory.

### Locating System Directories

func url(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, appropriateFor: URL?, create: Bool) throws -> URL

Locates and optionally creates the specified common directory in a domain.

func urls(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask) -> [URL]

Returns an array of URLs for the specified common directory in the requested domains.

func NSSearchPathForDirectoriesInDomains(FileManager.SearchPathDirectory, FileManager.SearchPathDomainMask, Bool) -> [String]

Creates a list of directory search paths.

