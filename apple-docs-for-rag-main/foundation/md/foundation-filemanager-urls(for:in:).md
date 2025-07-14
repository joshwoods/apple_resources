

- Foundation
- FileManager
-  urls(for:in:) 

Instance Method

# urls(for:in:)

Returns an array of URLs for the specified common directory in the requested domains.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urls(
    for directory: FileManager.SearchPathDirectory,
    in domainMask: FileManager.SearchPathDomainMask
) -> [URL]
```

## Parameters 

`directory`  

The search path directory. The supported values are described in FileManager.SearchPathDirectory.

`domainMask`  

The file system domain to search. The value for this parameter is one or more of the constants described in FileManager.SearchPathDomainMask.

## Return Value

An array of NSURL objects identifying the requested directories. The directories are ordered according to the order of the domain mask constants, with items in the user domain first and items in the system domain last.

## Discussion

This method is intended to locate known and common directories in the system. For example, setting the directory to FileManager.SearchPathDirectory.applicationDirectory, will return the Applications directories in the requested domain. There are a number of common directories available in the FileManager.SearchPathDirectory, including: FileManager.SearchPathDirectory.desktopDirectory, FileManager.SearchPathDirectory.applicationSupportDirectory, and many more.

## See Also

### Locating System Directories

func url(for: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, appropriateFor: URL?, create: Bool) throws -> URL

Locates and optionally creates the specified common directory in a domain.

func NSSearchPathForDirectoriesInDomains(FileManager.SearchPathDirectory, FileManager.SearchPathDomainMask, Bool) -> [String]

Creates a list of directory search paths.

func NSOpenStepRootDirectory() -> String

Returns the root directory of the user’s system.

