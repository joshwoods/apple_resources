

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Geometry
-  init(bounds:transform:) 

Initializer

# init(bounds:transform:)

Creates an instance with an optional bounding box and transform.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    bounds: BoundingBox = BoundingBox.empty,
    transform: Transform = Transform.identity
)
```

## Parameters 

`bounds`  

An optional bounding box to specify the size of the generated 3D model. If you don’t pass a value, the initializer sets the bounding box to .empty, which tells RealityKit to calculate the object’s size.

`transform`  

An optional Transform that RealityKit applies to the object after it’s created. Use this to scale, rotate, or move the object before the session publishes the PhotogrammetrySession.Output.requestComplete(_:_:)

