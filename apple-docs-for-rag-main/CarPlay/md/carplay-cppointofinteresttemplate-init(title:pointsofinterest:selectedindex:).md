

- CarPlay
- CPPointOfInterestTemplate
-  init(title:pointsOfInterest:selectedIndex:) 

Initializer

# init(title:pointsOfInterest:selectedIndex:)

Creates a Point of Interest template with a title, the points of interest to display, and the initial selection’s index.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    title: String,
    pointsOfInterest: [CPPointOfInterest],
    selectedIndex: Int
)
```

## Parameters 

`title`  

The scrollable picker’s title.

`pointsOfInterest`  

An array that contains the points of interest the template displays.

`selectedIndex`  

The initial selection’s index. This is the array’s index for the specific point of interest you want to select. Use NSNotFound to indicate no initial selection.

## Discussion

`pointsOfInterest` can contain a maximum of twelve points of interest because that is the most the template displays.

## See Also

### Creating a Point of Interest Template

class CPPointOfInterest

An object that describes a point of interest on the template’s map and in its scrollable picker.

