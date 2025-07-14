

- SceneKit
- SCNProgram
-  setSemantic(\_:forSymbol:options:) 

Instance Method

# setSemantic(\_:forSymbol:options:)

Associates a SceneKit semantic identifier with the specified GLSL vertex attribute or uniform variable.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func setSemantic(
    _ semantic: String?,
    forSymbol symbol: String,
    options: [String : Any]? = nil
)
```

## Parameters 

`semantic`  

A SceneKit semantic identifier. See Geometry Semantic Identifiers and Rendering Transform Keys for possible values.

`symbol`  

The name declared in the program’s GLSL source code for the vertex attribute or uniform variable to be associated with the semantic.

`options`  

A dictionary of options affecting the semantic. See `Program Semantic Options` for applicable keys and values.

## Discussion

Use this method to provide inputs managed by SceneKit to your GLSL program.

To use vertex attributes provided by SCNGeometry objects, use the constants listed in Geometry Semantic Identifiers.

To use the coordinate transformations defined by the scene’s node hierarchy and point-of-view camera, use the constants listed in Rendering Transform Keys.

## See Also

### Mapping GLSL Symbols to SceneKit Semantics

let SCNProgramMappingChannelKey: String

The mapping channel to be used for a texture coordinate semantic.

func semantic(forSymbol: String) -> String?

Returns the SceneKit semantic identifiers associated with the specified GLSL vertex attribute or uniform variable.

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

