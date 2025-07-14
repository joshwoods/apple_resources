

- AppKit
- NSImageView
-  isEditable 

Instance Property

# isEditable

A Boolean value indicating whether the user can drag a new image into the image view.

macOS

``` source
@MainActor
var isEditable: Bool { get set }
```

## Discussion

When the value of this property is true, the user can set the displayed image by dragging an image onto the image view. The default value of this property is false, which causes the image view to display only the programmatically set image.

## See Also

### Responding to user events

var allowsCutCopyPaste: Bool

A Boolean value indicating whether the image view lets the user cut, copy, and paste the image contents.

