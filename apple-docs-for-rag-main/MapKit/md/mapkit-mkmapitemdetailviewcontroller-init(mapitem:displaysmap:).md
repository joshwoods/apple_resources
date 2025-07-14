

- MapKit
- MKMapItemDetailViewController
-  init(mapItem:displaysMap:) 

Initializer

# init(mapItem:displaysMap:)

Create a map item detail view controller

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
init(
    mapItem: MKMapItem?,
    displaysMap: Bool
)
```

## Parameters 

`mapItem`  

The map item to display, or `nil` to indicate the item is loading.

`displaysMap`  

Specify `true` to display an inline map with the place information. Specify `false` only if the application is already displaying a map view elsewhere.

## See Also

### Creating a map item detail view controller

init(mapItem: MKMapItem?)

Create a map item detail view controller.

