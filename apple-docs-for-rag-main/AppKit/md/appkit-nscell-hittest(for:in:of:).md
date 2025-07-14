

- AppKit
- NSCell
-  hitTest(for:in:of:) 

Instance Method

# hitTest(for:in:of:)

Returns hit testing information for the receiver.

macOS 10.5+

``` source
@MainActor
func hitTest(
    for event: NSEvent,
    in cellFrame: NSRect,
    of controlView: NSView
) -> NSCell.HitResult
```

## Parameters 

`event`  

The current event.

`cellFrame`  

The cell’s frame.

`controlView`  

The control object in which the cell is located.

## Return Value

A constant that specifies the type of area in which the event occurred—see NSCell.HitResult for values.

## Discussion

You can use a bit-wise mask to look for a specific value when calling this method—see NSCell.HitResult for values.

Generally, this method should be overridden by custom `NSCell` subclasses to return the correct result. Currently, it is called by some multi-cell views, such as `NSTableView`.

By default, `NSCell` looks at the cell type and does the following:

- `NSImageCellType`: If the image exists and the event point is in the image returns `NSCellHitContentArea`, otherwise `NSCellHitNone`.

- `NSTextCellType` (also applies to `NSTextFieldCell`):

If there is text: If the event point hits in the text, return `NSCellHitContentArea`. Additionally, if the cell is enabled return `NSCellHitContentArea` `|` `NSCellHitEditableTextArea`.

If there is not text: return `NSCellHitNone`.

- `NSNullCellType` (this is the default that applies to non text or image cells who don’t override hitTest(for:in:of:)):

Return `NSCellHitContentArea` by default;

If the cell not disabled, and it would track, return `NSCellHitContentArea` `|` `NSCellHitTrackableArea`.

