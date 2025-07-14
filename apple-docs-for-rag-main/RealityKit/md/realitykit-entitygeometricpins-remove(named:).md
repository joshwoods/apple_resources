

- RealityKit
- EntityGeometricPins
-  remove(named:) 

Instance Method

# remove(named:)

Removes a geometric pin with the given name from this entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func remove(named name: String)
```

## Parameters 

`name`  

The name of the geometric pin to remove.

## Discussion

If found, the pin is removed from the entity’s GeometricPinsComponent. There is no effect if no matching GeometricPin is found.

