

- SceneKit
- SCNProgram
-  semantic(forSymbol:) 

Instance Method

# semantic(forSymbol:)

Returns the SceneKit semantic identifiers associated with the specified GLSL vertex attribute or uniform variable.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func semantic(forSymbol symbol: String) -> String?
```

## Parameters 

`symbol`  

The name declared in the program’s GLSL source code for a vertex attribute or uniform variable semantic.

## Return Value

A SceneKit semantic identifier. See Geometry Semantic Identifiers and Rendering Transform Keys for possible values.

## See Also

### Mapping GLSL Symbols to SceneKit Semantics

func setSemantic(String?, forSymbol: String, options: [String : Any]?)

Associates a SceneKit semantic identifier with the specified GLSL vertex attribute or uniform variable.

let SCNProgramMappingChannelKey: String

The mapping channel to be used for a texture coordinate semantic.

let SCNModelTransform: String

A 4 x 4 matrix for transforming coordinates from model space to scene (or world) space.

let SCNModelViewProjectionTransform: String

A 4 x 4 matrix containing the concatenation of the Model, View, and Projection transformations.

let SCNModelViewTransform: String

A 4 x 4 matrix containing the concatenation of the Model and View transformations.

let SCNNormalTransform: String

A 4 x 4 matrix for transforming surface normal vectors from model space to view (or eye) space.

let SCNProjectionTransform: String

A 4 x 4 matrix for transforming coordinates from view (or eye) space to clip space.

let SCNViewTransform: String

A 4 x 4 matrix for transforming coordinates from scene (or world) space to view (or eye) space.

