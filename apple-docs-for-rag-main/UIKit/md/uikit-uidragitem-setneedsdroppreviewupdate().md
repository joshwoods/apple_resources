

- UIKit
- UIDragItem
-  setNeedsDropPreviewUpdate() 

Instance Method

# setNeedsDropPreviewUpdate()

Notifies the operating system that an updated drop preview is available for the item.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+

``` source
@MainActor
func setNeedsDropPreviewUpdate()
```

## Discussion

Call this method to provide an updated drop preview after UIKit has started the drop animation. If the drop animation is still ongoing, UIKit calls the drop interaction delegate’s dropInteraction(_:previewForDropping:withDefault:) method, passing the previous drop preview as the `defaultPreview`.

## See Also

### Changing the drag item preview

var previewProvider: (() -> UIDragPreview?)?

A visual preview of the drag item, displayed while the user drags the item across the screen.

