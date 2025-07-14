

- CarPlay
- CPPointOfInterestTemplate
-  setPointsOfInterest(\_:selectedIndex:) 

Instance Method

# setPointsOfInterest(\_:selectedIndex:)

Updates the points of interest and the current selection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func setPointsOfInterest(
    _ pointsOfInterest: [CPPointOfInterest],
    selectedIndex: Int
)
```

## Parameters 

`pointsOfInterest`  

An array that contains the points of interest the template displays.

`selectedIndex`  

The selection’s index. This is the array’s index for the specific point of interest you want to select. Use NSNotFound to indicate no initial selection.

## Discussion

`pointsOfInterest` can contain a maximum of twelve points of interest because that is the most the template displays.

## See Also

### Managing the Points of Interest

var pointsOfInterest: [CPPointOfInterest]

The points of interest the template displays on the map and in the scrollable picker.

var selectedIndex: Int

The current selection’s index.

