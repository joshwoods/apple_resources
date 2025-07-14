

- Quick Look
- QLPreviewControllerDelegate
-  previewController(\_:transitionImageFor:contentRect:) 

Instance Method

# previewController(\_:transitionImageFor:contentRect:)

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewController(
    _ controller: QLPreviewController,
    transitionImageFor item: any QLPreviewItem,
    contentRect: UnsafeMutablePointer
) -> UIImage?
```

## Parameters 

`controller`  

The QLPreviewController that’s requesting the image for the preview item.

`item`  

The item to preview or dismiss.

`contentRect`  

The rectangle within the image that represents the document content. For icons, for example, the document content rectangle is typically smaller than the icon rectangle itself.

## Return Value

A UIImage object that the preview controller cross-fades with when zooming.

## Discussion

Note

Starting with macOS 11, animated transitions are available for Mac apps built with Mac Catalyst. On Mac computers running a version earlier than macOS 11, the system doesn’t call this delegate method.

## See Also

### Responding to preview requests

func previewController(QLPreviewController, frameFor: any QLPreviewItem, inSourceView: AutoreleasingUnsafeMutablePointer&lt;UIView?>) -> CGRect

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a zoom effect.

func previewController(QLPreviewController, transitionViewFor: any QLPreviewItem) -> UIView?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewControllerWillDismiss(QLPreviewController)

Tells the delegate that the preview is about to close.

func previewControllerDidDismiss(QLPreviewController)

Tells the delegate that the preview was closed.

