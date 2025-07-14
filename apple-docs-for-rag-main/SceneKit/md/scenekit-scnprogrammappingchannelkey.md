

- SceneKit
-  SCNProgramMappingChannelKey 

Global Variable

# SCNProgramMappingChannelKey

The mapping channel to be used for a texture coordinate semantic.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
let SCNProgramMappingChannelKey: String
```

## Discussion

This key can be used with the `options` dictionary for the setSemantic(_:forSymbol:options:) method, and applies only to the texcoord semantic. Its value is an NSNumber object containing an unsigned integer value.

A geometry can provide, and a shader program can use, more than one source of texture coordinates for each vertex. Use this key to specify which geometry source should provide data for each texture sampler vertex attribute declared in a shader program. The mapping channel for a geometry source corresponds to its index in the array returned by calling the sources(for:) method.

## See Also

### Mapping GLSL Symbols to SceneKit Semantics

func setSemantic(String?, forSymbol: String, options: [String : Any]?)

Associates a SceneKit semantic identifier with the specified GLSL vertex attribute or uniform variable.

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

