

- AppKit
- NSTabViewItem
-  drawLabel(\_:in:) 

Instance Method

# drawLabel(\_:in:)

Draws the receiver’s label in `tabRect`, which is the area between the curved end caps.

macOS

``` source
func drawLabel(
    _ shouldTruncateLabel: Bool,
    in labelRect: NSRect
)
```

## Discussion

If `shouldTruncateLabel` is false, draws the full label in the rectangle specified by `tabRect`. If `shouldTruncateLabel` is true, draws the truncated label. You can override this method to perform customized label drawing. For example, you might want to add an icon to each tab in the view.

## See Also

### Working with Labels

var label: String

Sets the label text for the receiver to `label`.

func sizeOfLabel(Bool) -> NSSize

Calculates the size of the receiver’s label.

