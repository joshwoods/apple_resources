

- CarPlay
- CPTrip
-  destinationNameVariants 

Instance Property

# destinationNameVariants

An array of strings that represents the names of the destination for this trip, arranged from most to least preferred.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var destinationNameVariants: [String]? { get set }
```

## Discussion

You need to provide at least one variant. Present the variant strings as localized, displayable content.

## See Also

### Getting Route Choices

var routeChoices: [CPRouteChoice]

The list of route choices for the trip.

