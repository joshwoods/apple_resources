

- CarPlay
- CPPointOfInterestTemplate
-  pointsOfInterest 

Instance Property

# pointsOfInterest

The points of interest the template displays on the map and in the scrollable picker.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var pointsOfInterest: [CPPointOfInterest] { get }
```

## Discussion

You must call the setPointsOfInterest(_:selectedIndex:) method to update the points of interest the template displays.

## See Also

### Managing the Points of Interest

func setPointsOfInterest([CPPointOfInterest], selectedIndex: Int)

Updates the points of interest and the current selection.

var selectedIndex: Int

The current selection’s index.

