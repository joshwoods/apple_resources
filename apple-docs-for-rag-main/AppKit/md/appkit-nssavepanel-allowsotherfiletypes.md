

- AppKit
- NSSavePanel
-  allowsOtherFileTypes 

Instance Property

# allowsOtherFileTypes

A Boolean value that indicates whether the panel allows the user to save files with a filename extension that’s not in the list of allowed types.

macOS

``` source
@MainActor
var allowsOtherFileTypes: Bool { get set }
```

## Discussion

When the value of this property is true, the panel allows the user to save files with an extension that’s not in the list of allowed types. The default value is false.

If the user tries to save a filename with a recognized extension that’s not in the list of allowed types, they are presented with a dialog. If the value of this property is true, then the dialog presents the option of using the extension the user specified.

## See Also

### Configuring the File Types

var allowedContentTypes: [UTType]

An array of types that specify the files types to which you can save.

var treatsFilePackagesAsDirectories: Bool

A Boolean value that indicates whether the panel displays file packages as directories.

