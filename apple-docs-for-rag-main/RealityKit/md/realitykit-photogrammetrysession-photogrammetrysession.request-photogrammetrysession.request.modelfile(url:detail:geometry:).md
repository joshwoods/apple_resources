

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.modelFile(url:detail:geometry:) 

Case

# PhotogrammetrySession.Request.modelFile(url:detail:geometry:)

An object-creation request saved to a USDZ file or a folder (for OBJ output).

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case modelFile(
    url: URL,
    detail: PhotogrammetrySession.Request.Detail = .reduced,
    geometry: PhotogrammetrySession.Request.Geometry? = nil
)
```

## Parameters 

`url`  

The location URL in the file system where you want to save the model file. The request saves a USDZ file if the `url` ends with `.usdz`. If `url` refers to a directory, the request saves an OBJ object and every texture map there.

`detail`  

The level of detail for the created model.

`geometry`  

The bounding box or transforms for the generated object.

## See Also

### Specifying the output

case modelEntity(detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request stored in-memory for immediate display.

case bounds

An object-creation request that returns a box the same size as the created model.

enum Detail

Supported levels of detail for a request.

