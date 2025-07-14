

- Quick Look
- QLPreviewControllerDelegate
-  previewControllerDidDismiss(\_:) 

Instance Method

# previewControllerDidDismiss(\_:)

Tells the delegate that the preview was closed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func previewControllerDidDismiss(_ controller: QLPreviewController)
```

## Parameters 

`controller`  

The QLPreviewController that just closed.

## See Also

### Responding to preview requests

func previewController(QLPreviewController, frameFor: any QLPreviewItem, inSourceView: AutoreleasingUnsafeMutablePointer&lt;UIView?>) -> CGRect

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a zoom effect.

func previewController(QLPreviewController, transitionImageFor: any QLPreviewItem, contentRect: UnsafeMutablePointer&lt;CGRect>) -> UIImage?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewController(QLPreviewController, transitionViewFor: any QLPreviewItem) -> UIView?

Tells the delegate that the system is about to present the preview full screen or dismiss it, and asks for information to provide a smooth transition when zooming.

func previewControllerWillDismiss(QLPreviewController)

Tells the delegate that the preview is about to close.

