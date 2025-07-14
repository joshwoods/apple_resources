

- MapKit
- MKMapItemDetailViewController
-  init(mapItem:) 

Initializer

# init(mapItem:)

Create a map item detail view controller.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
init(mapItem: MKMapItem?)
```

## Parameters 

`mapItem`  

The map item to display, or `nil` to indicate the item is loading.

## Discussion

Displays an inline map with the place data.

## See Also

### Creating a map item detail view controller

init(mapItem: MKMapItem?, displaysMap: Bool)

Create a map item detail view controller

