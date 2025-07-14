

- AppKit
- NSTabViewItem
-  sizeOfLabel(\_:) 

Instance Method

# sizeOfLabel(\_:)

Calculates the size of the receiver’s label.

macOS

``` source
func sizeOfLabel(_ computeMin: Bool) -> NSSize
```

## Discussion

If `shouldTruncateLabel` is false, returns the size of the receiver’s full label. If `shouldTruncateLabel` is true, returns the truncated size. If your application does anything to change the size of tab labels, such as overriding the drawLabel(_:in:) method to add an icon to each tab, you should override sizeOfLabel(_:) too so the NSTabView knows the correct size for the tab label.

## See Also

### Related Documentation

var font: NSFont

The font used for the tab view’s label text.

### Working with Labels

func drawLabel(Bool, in: NSRect)

Draws the receiver’s label in `tabRect`, which is the area between the curved end caps.

var label: String

Sets the label text for the receiver to `label`.

