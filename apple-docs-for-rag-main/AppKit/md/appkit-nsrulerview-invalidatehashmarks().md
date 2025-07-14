

- AppKit
- NSRulerView
-  invalidateHashMarks() 

Instance Method

# invalidateHashMarks()

Forces recalculation of the hash mark spacing for the next time the receiver is displayed.

macOS

``` source
@MainActor
func invalidateHashMarks()
```

## Discussion

You should never need to invoke this method directly, but might need to override it if you override drawHashMarksAndLabels(in:).

## See Also

### Drawing

func drawHashMarksAndLabels(in: NSRect)

Draws the receiver’s hash marks and labels in `aRect`, which is expressed in the receiver’s coordinate system.

func drawMarkers(in: NSRect)

Draws the receiver’s markers in `aRect`, which is expressed in the receiver’s coordinate system.

