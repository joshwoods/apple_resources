

- RealityKit
- Entity
-  align(\_:to:) 

Instance Method

# align(\_:to:)

Moves and rotates the entity by a transformation from the origin pin to the target pin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult @MainActor @preconcurrency
func align(
    _ originPin: GeometricPin,
    to targetPin: GeometricPin
) -> float4x4?
```

## Parameters 

`originPin`  

The `GeometricPin` to align. It should be one of the pins on the entity.

`targetPin`  

The `GeometricPin` to align to.

## Return Value

Transformation matrix that has been applied to the `Entity`, in the frame or reference of the parent of the `Entity`. If either pin doesn’t exist, returns `nil`.

