

- AppKit
- NSRulerView
-  drawHashMarksAndLabels(in:) 

Instance Method

# drawHashMarksAndLabels(in:)

Draws the receiver’s hash marks and labels in `aRect`, which is expressed in the receiver’s coordinate system.

macOS

``` source
@MainActor
func drawHashMarksAndLabels(in rect: NSRect)
```

## Discussion

This method is invoked by draw(_:)—you should never need to invoke it directly. You can define custom measurement units using the class method registerUnit(withName:abbreviation:unitToPointsConversionFactor:stepUpCycle:stepDownCycle:). Override this method if you want to customize the appearance of the hash marks themselves.

## See Also

### Drawing

func drawMarkers(in: NSRect)

Draws the receiver’s markers in `aRect`, which is expressed in the receiver’s coordinate system.

func invalidateHashMarks()

Forces recalculation of the hash mark spacing for the next time the receiver is displayed.

