

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.modelEntity(detail:geometry:) 

Case

# PhotogrammetrySession.Request.modelEntity(detail:geometry:)

An object-creation request stored in-memory for immediate display.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case modelEntity(
    detail: PhotogrammetrySession.Request.Detail = .reduced,
    geometry: PhotogrammetrySession.Request.Geometry? = nil
)
```

## Parameters 

`detail`  

The level of detail for the created model.

`geometry`  

The bounding box and transforms for the entity the request generates.

## See Also

### Specifying the output

case modelFile(url: URL, detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request saved to a USDZ file or a folder (for OBJ output).

case bounds

An object-creation request that returns a box the same size as the created model.

enum Detail

Supported levels of detail for a request.

