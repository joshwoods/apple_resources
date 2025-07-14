

- AppKit
- NSLayoutManager
-  showAttachmentCell(\_:in:characterIndex:) 

Instance Method

# showAttachmentCell(\_:in:characterIndex:)

Draws an attachment cell.

macOS 10.7+

``` source
func showAttachmentCell(
    _ cell: NSCell,
    in rect: NSRect,
    characterIndex attachmentIndex: Int
)
```

## Parameters 

`cell`  

The attachment cell to draw.

`rect`  

The rectangle within which to draw `cell`.

`attachmentIndex`  

The location of the attachment cell.

## Discussion

The `attachmentIndex` parameter is provided for cells that alter their appearance based on their location.

## See Also

### Managing attachments

var defaultAttachmentScaling: NSImageScaling

The default amount of scaling to apply when an attachment image is too large to fit in a text container.

