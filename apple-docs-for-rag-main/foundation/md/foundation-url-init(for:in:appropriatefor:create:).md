

- Foundation
- URL
-  init(for:in:appropriateFor:create:) 

Initializer

# init(for:in:appropriateFor:create:)

Creates a file URL for a common directory in a domain.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    for directory: FileManager.SearchPathDirectory,
    in domain: FileManager.SearchPathDomainMask,
    appropriateFor url: URL? = nil,
    create shouldCreate: Bool = false
) throws
```

## Parameters 

`directory`  

The search path for the commonly used directory, such as FileManager.SearchPathDirectory.desktopDirectory or FileManager.SearchPathDirectory.downloadsDirectory.

`domain`  

The file system domain to search, which the values in FileManager.SearchPathDomainMask define. Specify only one domain for this parameter. You may not specify allDomainsMask with this initializer.

`url`  

The file URL for determining the location of the returned URL. Only the volume of this parameter is relevant.

The initializer ignores this parameter unless the directory parameter contains the value FileManager.SearchPathDirectory.itemReplacementDirectory and the domain parameter contains the value userDomainMask.

`shouldCreate`  

A Boolean value that indicates whether the initializer creates the directory if it doesn’t already exist.

## See Also

### Creating a file URL for a common directory

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

