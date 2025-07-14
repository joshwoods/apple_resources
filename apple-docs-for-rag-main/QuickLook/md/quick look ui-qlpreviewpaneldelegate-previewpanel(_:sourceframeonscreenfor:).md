

- Quick Look UI
- QLPreviewPanelDelegate
-  previewPanel(\_:sourceFrameOnScreenFor:) 

Instance Method

# previewPanel(\_:sourceFrameOnScreenFor:)

Returns the screen rectangle for a given preview item.

macOS 10.6+

``` source
optional func previewPanel(
    _ panel: QLPreviewPanel!,
    sourceFrameOnScreenFor item: (any QLPreviewItem)!
) -> NSRect
```

## Parameters 

`panel`  

The preview panel.

`item`  

The preview item for which the screen rectangle is required.

## Return Value

The screen rectangle for the given preview item. Return NSZeroRect if there is no origin point (this will produce a fade of the panel).

## Discussion

The system invokes this optional method when the preview panel opens or closes to provide a zoom effect. You should return — in screen coordinates — the rectangle that displays the specified preview item.

## See Also

### Optional Methods

func previewPanel(QLPreviewPanel!, handle: NSEvent!) -> Bool

Handles an event that the preview panel receives, but doesn’t handle.

func previewPanel(QLPreviewPanel!, transitionImageFor: (any QLPreviewItem)!, contentRect: UnsafeMutablePointer&lt;NSRect>!) -> Any!

Returns the image to use for the transition zoom effect for a given item.

