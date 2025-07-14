

- AppKit
- NSCell
-  draggingImageComponents(withFrame:in:) 

Instance Method

# draggingImageComponents(withFrame:in:)

Generates dragging image components with the specified frame in the view.

macOS 10.7+

``` source
@MainActor
func draggingImageComponents(
    withFrame frame: NSRect,
    in view: NSView
) -> [NSDraggingImageComponent]
```

## Parameters 

`frame`  

The bounding rectangle of the receiver.

`view`  

The view that manages the cell.

## Return Value

An array of NSDraggingImageComponent objects representing the cell.

## Discussion

The default implementation generates an image from the cell and return two components: one for label and another for icon. This is done by capturing the portion from the titleRect(forBounds:) and imageRect(forBounds:) methods respectively.

This method can be subclassed and overridden to provide a custom set of NSDraggingImageComponent to create the drag image for the cell. This method is generally used by NSTableView/NSOutlineView.

Note

NSCell currently has an issue where it will return an empty array from `draggingImageComponentsWithFrame:inView:` if the cell does not have an image portion. To work around this, subclass NSCell and override `draggingImageComponentsWithFrame:inView:` and generate your own NSDraggingImageComponent in the returned array.

