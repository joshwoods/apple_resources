

- AppKit
- NSSavePanel
-  treatsFilePackagesAsDirectories 

Instance Property

# treatsFilePackagesAsDirectories

A Boolean value that indicates whether the panel displays file packages as directories.

macOS

``` source
@MainActor
var treatsFilePackagesAsDirectories: Bool { get set }
```

## Discussion

When the value of this property is true, the panel displays file packages as directories; if false, it will not.

## See Also

### Configuring the File Types

var allowedContentTypes: [UTType]

An array of types that specify the files types to which you can save.

var allowsOtherFileTypes: Bool

A Boolean value that indicates whether the panel allows the user to save files with a filename extension that’s not in the list of allowed types.

