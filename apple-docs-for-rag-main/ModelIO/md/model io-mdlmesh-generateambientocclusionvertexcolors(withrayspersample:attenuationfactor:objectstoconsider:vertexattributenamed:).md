

- Model I/O
- MDLMesh
-  generateAmbientOcclusionVertexColors(withRaysPerSample:attenuationFactor:objectsToConsider:vertexAttributeNamed:) 

Instance Method

# generateAmbientOcclusionVertexColors(withRaysPerSample:attenuationFactor:objectsToConsider:vertexAttributeNamed:)

Calculates ambient occlusion (AO) information for the mesh, using the specified number of rays per sample, and saves it in the mesh as a vertex color attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func generateAmbientOcclusionVertexColors(
    withRaysPerSample raysPerSample: Int,
    attenuationFactor: Float,
    objectsToConsider: [MDLObject],
    vertexAttributeNamed vertexAttributeName: String
) -> Bool
```

## Parameters 

`raysPerSample`  

The number of rays to trace for vertex in the mesh to test for potential occlusion. Higher numbers produce more accurate output at the cost of more processing time and memory usage.

`attenuationFactor`  

A value between `0.0` and `1.0` that scales the strength of the AO effect. Higher values result in higher contrast when the AO color data is used for shading.

`objectsToConsider`  

An array of other objects in the scene that should affect static ambient lighting for the mesh.

`vertexAttributeName`  

The name of the vertex attribute for storing generated vertex color data.

## Return Value

true if AO calculation succeeded; otherwise false.

## Discussion

Ambient occlusion (AO) is a measure, for each point on a surface, of how much ambient light can reach that point. For example, a narrow, concave section of a mesh does not receive much ambient light compared with a wide, flat section—thus, in a realistic rendering of the mesh, the concave sections should appear darker than the flat sections. This method analyzes the mesh (and, optionally, static elements of its local environment, specified in the `objectsToConsider` parameter) to precompute (or “bake”) AO information for each point on the mesh’s surface. You can then use the resulting information in shading to produce a more realistic render.

This method saves AO data as per-vertex colors. Using vertex colors to modulate shading can result in similar results without the texture memory and vertex attribute overhead of a texture map, but the fidelity of this effect depends on the vertex complexity of the mesh. Vertex colors are saved in the vertex attribute specified in the `vertexAttributeName` parameter. If the mesh already contains that attribute, this method overwrites the contents of the corresponding vertex buffer. If the mesh does not contain that attribute, this method creates a new attribute and updates the mesh’s vertexDescriptor object accordingly.

The `raysPerSample` parameter controls the fidelity and performance of the AO calculation process and its output. To control quality without specifying raytracing options, use the generateAmbientOcclusionVertexColors(withQuality:attenuationFactor:objectsToConsider:vertexAttributeNamed:) method.

## See Also

### Generating Ambient Occlusion Data

func generateAmbientOcclusionTexture(withQuality: Float, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a material property texture.

func generateAmbientOcclusionTexture(withSize: vector_int2, raysPerSample: Int, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a material property texture of the specified size.

func generateAmbientOcclusionVertexColors(withQuality: Float, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a vertex color attribute.

