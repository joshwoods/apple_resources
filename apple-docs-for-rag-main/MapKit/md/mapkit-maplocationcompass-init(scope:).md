

- MapKit
- MapLocationCompass
-  init(scope:) 

Initializer

# init(scope:)

Creates a new map location compass with the provided scope.

MapKitSwiftUIwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(scope: Namespace.ID? = nil)
```

## Parameters 

`scope`  

The namespace the framework passes to the associated Map and `MapLocationCompass/mapScope(_:)`. For use outside of `MapLocationCompass/mapControls(_:)`.

## Discussion

