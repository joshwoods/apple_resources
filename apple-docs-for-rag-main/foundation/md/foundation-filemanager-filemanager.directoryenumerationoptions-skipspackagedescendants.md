

- Foundation
- FileManager
- FileManager.DirectoryEnumerationOptions
-  skipsPackageDescendants 

Type Property

# skipsPackageDescendants

An option to treat packages like files and not descend into their contents.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var skipsPackageDescendants: FileManager.DirectoryEnumerationOptions { get }
```

## See Also

### Directory Enumeration Options

static var skipsSubdirectoryDescendants: FileManager.DirectoryEnumerationOptions

An option to perform a shallow enumeration that doesn’t descend into directories.

static var skipsHiddenFiles: FileManager.DirectoryEnumerationOptions

An option to skip hidden files.

