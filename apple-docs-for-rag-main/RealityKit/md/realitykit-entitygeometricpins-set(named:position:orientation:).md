

- RealityKit
- EntityGeometricPins
-  set(named:position:orientation:) 

Instance Method

# set(named:position:orientation:)

Creates and adds a geometric pin to the entity, and returns the entity geometric pin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult @MainActor
func set(
    named name: String,
    position: SIMD3 = SIMD3(0, 0, 0),
    orientation: simd_quatf = simd_quatf(ix: 0, iy: 0, iz: 0, r: 1)
) -> GeometricPin
```

## Parameters 

`name`  

The name of the pin in the namespace of the owning entity.

`position`  

The position of the pin, in local space of the owning entity.

`orientation`  

The orientation of the pin, in local space of the owning entity.

## Return Value

A `GeometricPin`, identifying the newly added reference frame on the Entity.

## Discussion

The pin is added to the entity’s GeometricPinsComponent.

