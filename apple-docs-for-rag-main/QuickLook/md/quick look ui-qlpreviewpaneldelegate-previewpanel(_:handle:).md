

- Quick Look UI
- QLPreviewPanelDelegate
-  previewPanel(\_:handle:) 

Instance Method

# previewPanel(\_:handle:)

Handles an event that the preview panel receives, but doesn’t handle.

macOS 10.6+

``` source
optional func previewPanel(
    _ panel: QLPreviewPanel!,
    handle event: NSEvent!
) -> Bool
```

## Parameters 

`panel`  

The preview panel.

`event`  

The event that the preview panel wasn’t able to handle.

## Return Value

true if the receiver handled the event; otherwise, false.

## Discussion

The preview panel invokes this optional method when it receives an event it doesn’t handle.

## See Also

### Optional Methods

func previewPanel(QLPreviewPanel!, sourceFrameOnScreenFor: (any QLPreviewItem)!) -> NSRect

Returns the screen rectangle for a given preview item.

func previewPanel(QLPreviewPanel!, transitionImageFor: (any QLPreviewItem)!, contentRect: UnsafeMutablePointer&lt;NSRect>!) -> Any!

Returns the image to use for the transition zoom effect for a given item.

