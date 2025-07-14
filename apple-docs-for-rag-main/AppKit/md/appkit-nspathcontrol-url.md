

- AppKit
- NSPathControl
-  url 

Instance Property

# url

The path value displayed by the receiver.

macOS 10.5+

``` source
@MainActor
var url: URL? { get set }
```

## Discussion

When setting, an array of `NSPathComponentCell` objects is automatically set based on the path in `url`. If `url` is a file URL (returns true from isFileURL), the images are automatically filled with file icons, if the path exists. The URL value itself is stored in the `objectValue` property of the cell.

