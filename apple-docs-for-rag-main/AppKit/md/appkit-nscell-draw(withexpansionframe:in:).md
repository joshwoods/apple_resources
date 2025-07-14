

- AppKit
- NSCell
-  draw(withExpansionFrame:in:) 

Instance Method

# draw(withExpansionFrame:in:)

Instructs the receiver to draw in an expansion frame.

macOS 10.5+

``` source
@MainActor
func draw(
    withExpansionFrame cellFrame: NSRect,
    in view: NSView
)
```

## Parameters 

`cellFrame`  

The frame in which to draw.

`view`  

The view in which to draw. This view may be different from the original view that the cell appeared in.

## Discussion

This method allows the cell to perform custom expansion tool tip drawing. By default, `NSCell` simply calls draw(withFrame:in:).

## See Also

### Managing Expansion Frames

func expansionFrame(withFrame: NSRect, in: NSView) -> NSRect

Returns the expansion cell frame for the receiver.

