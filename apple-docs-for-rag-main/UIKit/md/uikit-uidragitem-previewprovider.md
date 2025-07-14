

- UIKit
- UIDragItem
-  previewProvider 

Instance Property

# previewProvider

A visual preview of the drag item, displayed while the user drags the item across the screen.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var previewProvider: (() -> UIDragPreview?)? { get set }
```

## Discussion

As the user drags an item across the screen, the system displays a preview. You can change the preview by setting previewProvider to a block that returns a UIDragPreview object. The system invokes the block if and when it needs the drag item preview.

To use the default preview, set previewProvider to `nil`. To hide the preview, set previewProvider to a block that returns `nil`.

## See Also

### Changing the drag item preview

func setNeedsDropPreviewUpdate()

Notifies the operating system that an updated drop preview is available for the item.

