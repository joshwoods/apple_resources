

- SpriteKit
- SKPhysicsWorld
-  sampleFields(at:) 

Instance Method

# sampleFields(at:)

Samples all of the field nodes in the scene and returns the summation of their forces at that point.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func sampleFields(at position: vector_float3) -> vector_float3
```

## Parameters 

`position`  

A position in scene coordinates.

## Return Value

The summation of forces exerted on that point.

## Discussion

The sample is calculated as if a physics body is placed at that position in the scene. The body is assumed to have a mass of `1.0`, with no charge or velocity. The body is affected by all field nodes.

