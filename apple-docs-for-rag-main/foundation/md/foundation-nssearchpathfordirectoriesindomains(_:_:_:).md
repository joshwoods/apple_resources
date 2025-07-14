

- Foundation
-  NSSearchPathForDirectoriesInDomains(\_:\_:\_:) 

Function

# NSSearchPathForDirectoriesInDomains(\_:\_:\_:)

Creates a list of directory search paths.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSSearchPathForDirectoriesInDomains(
    _ directory: FileManager.SearchPathDirectory,
    _ domainMask: FileManager.SearchPathDomainMask,
    _ expandTilde: Bool
) -> [String]
```

## Discussion

Creates a list of path strings for the specified directories in the specified domains. The list is in the order in which you should search the directories. If `expandTilde` is true, tildes are expanded as described in expandingTildeInPath.

You should consider using the FileManager methods urls(for:in:) and url(for:in:appropriateFor:create:). which return URLs, which are the preferred format.

For more information on file system utilities, see File System Programming Guide.

Note

The directory returned by this method may not exist. This method simply gives you the appropriate location for the requested directory. Depending on the application’s needs, it may be up to the developer to create the appropriate directory and any in between.

## See Also

### Locating System Directories

func url(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, appropriateFor: URL?, create: Bool) throws -> URL

Locates and optionally creates the specified common directory in a domain.

func urls(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask) -> [URL]

Returns an array of URLs for the specified common directory in the requested domains.

func NSOpenStepRootDirectory() -> String

Returns the root directory of the user’s system.

