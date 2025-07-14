

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.bounds 

Case

# PhotogrammetrySession.Request.bounds

An object-creation request that returns a box the same size as the created model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case bounds
```

## Discussion

Use a `bounds` request to quickly retrieve a box the same size as the final created object.

## See Also

### Specifying the output

case modelFile(url: URL, detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request saved to a USDZ file or a folder (for OBJ output).

case modelEntity(detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request stored in-memory for immediate display.

enum Detail

Supported levels of detail for a request.

