

- AppKit
- NSImageView
-  allowsCutCopyPaste 

Instance Property

# allowsCutCopyPaste

A Boolean value indicating whether the image view lets the user cut, copy, and paste the image contents.

macOS

``` source
@MainActor
var allowsCutCopyPaste: Bool { get set }
```

## Discussion

When the value of this property is YES, the user can cut, copy, or paste the image in the image view.

## See Also

### Responding to user events

var isEditable: Bool

A Boolean value indicating whether the user can drag a new image into the image view.

