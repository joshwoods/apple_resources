

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  maximumPolygonCount 

Instance Property

# maximumPolygonCount

The upper limit on polygons in the model mesh.

Mac Catalyst 17.0+macOS 14.0+

``` source
var maximumPolygonCount: UInt
```

## Discussion

Note: this is an upper bound to control the amount of decimation performed on complicated meshes to allow the user to target specific renderer resource budgets, and not a specification for how many polygons to use. Specifically, for less complex models, the actual number of polygons may be significantly less than this value – the algorithm will use as many as it deems necessary (within this limit) to accurately represent the reconstructed model.

