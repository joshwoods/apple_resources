

- AppKit
- NSSavePanel
-  allowedContentTypes 

Instance Property

# allowedContentTypes

An array of types that specify the files types to which you can save.

macOS 11.0+

``` source
@MainActor
var allowedContentTypes: [UTType] { get set }
```

## Discussion

Defaults to an empty array that indicates that you can use any file type. If you don’t provide an extension, the system uses the first preferred extension in the array for the save panel. If you specify a type that isn’t in the array and allowsOtherFileTypes is `YES`, the system presents another dialog when prompting you to save.

## See Also

### Configuring the File Types

var allowsOtherFileTypes: Bool

A Boolean value that indicates whether the panel allows the user to save files with a filename extension that’s not in the list of allowed types.

var treatsFilePackagesAsDirectories: Bool

A Boolean value that indicates whether the panel displays file packages as directories.

