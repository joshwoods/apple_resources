

- MapKit
- MKMapItemAnnotation
-  init(mapItem:) 

Initializer

# init(mapItem:)

Creates a map item annotation

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init?(mapItem: MKMapItem)
```

## Parameters 

`mapItem`  

The map item this annotation will represent

## Discussion

If the map item does not have valid coordinate data, the result will be nil.

