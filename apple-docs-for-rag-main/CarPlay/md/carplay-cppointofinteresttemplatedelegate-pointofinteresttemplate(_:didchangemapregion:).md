

- CarPlay
- CPPointOfInterestTemplateDelegate
-  pointOfInterestTemplate(\_:didChangeMapRegion:) 

Instance Method

# pointOfInterestTemplate(\_:didChangeMapRegion:)

Tells the delegate about changes to the visible region of the template’s map.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func pointOfInterestTemplate(
    _ pointOfInterestTemplate: CPPointOfInterestTemplate,
    didChangeMapRegion region: MKCoordinateRegion
)
```

**Required**

## Parameters 

`region`  

The map’s new visible region.

## Discussion

CarPlay calls this method whenever the user pans the template’s map and its visible region changes. In response, re-evaluate which points of interest are relevant to the new region and, if necessary, call setPointsOfInterest(_:selectedIndex:) to update the template.

