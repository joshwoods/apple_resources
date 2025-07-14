

- CarPlay
- CPPointOfInterestTemplate
-  selectedIndex 

Instance Property

# selectedIndex

The current selection’s index.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var selectedIndex: Int { get set }
```

## Discussion

The value of the property must be within the bounds of the pointsOfInterest array, or NSNotFound to indicate no selection.

## See Also

### Managing the Points of Interest

var pointsOfInterest: [CPPointOfInterest]

The points of interest the template displays on the map and in the scrollable picker.

func setPointsOfInterest([CPPointOfInterest], selectedIndex: Int)

Updates the points of interest and the current selection.

