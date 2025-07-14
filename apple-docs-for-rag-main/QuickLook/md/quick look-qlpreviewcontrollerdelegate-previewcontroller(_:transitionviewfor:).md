

- Quick Look
- QLPreviewControllerDelegate
-  previewController(\_:transitionViewFor:) 

Instance Method

# previewController(\_:transitionViewFor:)

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewController(
    _ controller: QLPreviewController,
    transitionViewFor item: any QLPreviewItem
) -> UIView?
```

## Parameters 

`controller`  

The QLPreviewController that’s requesting the view for the preview item.

`item`  

The item to preview or dismiss.

## Return Value

A UIView object that the preview controller cross-fades with when zooming.

## Discussion

Starting with macOS 11, animated transitions are available for Mac apps built with Mac Catalyst. On Mac computers running a version earlier than macOS 11, the system doesn’t call this delegate method.

## See Also

### Responding to preview requests

func previewController(QLPreviewController, frameFor: any QLPreviewItem, inSourceView: AutoreleasingUnsafeMutablePointer&lt;UIView?>) -> CGRect

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a zoom effect.

func previewController(QLPreviewController, transitionImageFor: any QLPreviewItem, contentRect: UnsafeMutablePointer&lt;CGRect>) -> UIImage?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewControllerWillDismiss(QLPreviewController)

Tells the delegate that the preview is about to close.

func previewControllerDidDismiss(QLPreviewController)

Tells the delegate that the preview was closed.

