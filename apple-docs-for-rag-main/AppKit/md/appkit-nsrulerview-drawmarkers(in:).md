

- AppKit
- NSRulerView
-  drawMarkers(in:) 

Instance Method

# drawMarkers(in:)

Draws the receiver’s markers in `aRect`, which is expressed in the receiver’s coordinate system.

macOS

``` source
@MainActor
func drawMarkers(in rect: NSRect)
```

## Discussion

This method is invoked by draw(_:); you should never need to invoke it directly, but you might want to override it if you want to do something different when drawing markers.

## See Also

### Related Documentation

var reservedThicknessForMarkers: CGFloat

The room available for ruler markers to `thickness`.

### Drawing

func drawHashMarksAndLabels(in: NSRect)

Draws the receiver’s hash marks and labels in `aRect`, which is expressed in the receiver’s coordinate system.

func invalidateHashMarks()

Forces recalculation of the hash mark spacing for the next time the receiver is displayed.

