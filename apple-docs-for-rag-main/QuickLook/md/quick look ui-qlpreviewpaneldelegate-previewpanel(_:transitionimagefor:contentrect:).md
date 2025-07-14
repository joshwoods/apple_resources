

- Quick Look UI
- QLPreviewPanelDelegate
-  previewPanel(\_:transitionImageFor:contentRect:) 

Instance Method

# previewPanel(\_:transitionImageFor:contentRect:)

Returns the image to use for the transition zoom effect for a given item.

macOS 10.6+

``` source
optional func previewPanel(
    _ panel: QLPreviewPanel!,
    transitionImageFor item: (any QLPreviewItem)!,
    contentRect: UnsafeMutablePointer!
) -> Any!
```

## Parameters 

`panel`  

The preview panel.

`item`  

The item the system is previewing.

`contentRect`  

The rectangle within a preview image that actually represents the content of the document. For icons, the actual rectangle is typically smaller than the icon itself.

## Return Value

The image to use for the transition zoom effect for the `item`.

## Discussion

The system invokes this optional method when the preview panel opens or closes to provide a smooth transition when zooming. The return type of the function should be an instance of NSImage.

## See Also

### Optional Methods

func previewPanel(QLPreviewPanel!, handle: NSEvent!) -> Bool

Handles an event that the preview panel receives, but doesn’t handle.

func previewPanel(QLPreviewPanel!, sourceFrameOnScreenFor: (any QLPreviewItem)!) -> NSRect

Returns the screen rectangle for a given preview item.

