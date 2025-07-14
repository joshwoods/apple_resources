

- SceneKit
- SCNGeometry
-  init(sources:elements:) 

Initializer

# init(sources:elements:)

Creates a new geometry built from the specified geometry sources and elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    sources: [SCNGeometrySource],
    elements: [SCNGeometryElement]?
)
```

## Parameters 

`sources`  

An array of SCNGeometrySource objects describing vertices in the geometry and their attributes.

`elements`  

An array of SCNGeometryElement objects describing how to connect the geometry’s vertices.

## Discussion

A geometry’s visible content comes from the combination of geometry sources, which contain data describing its vertices, with geometry elements, which contain data describing how the vertices connect to form a surface.

Each SCNGeometrySource object describes an attribute of all vertices in the geometry (vertex position, surface normal vector, color, or texture mapping coordinates) identified by the source’s semantic property. To create a custom geometry you must provide at least one source, for the vertex semantic. Typically, you also provide sources for normals and texture coordinates for use in lighting and shading.

Sources for the vertex, normal, and color semantics must be unique—if multiple objects in the `sources` array have the same semantic, SceneKit uses only the first. A geometry may have multiple sources for the texcoord semantic—the order of texture coordinate sources in the `sources` array determines the value to use for the mappingChannel property when attaching materials.

Each SCNGeometryElement object describes how vertices from the geometry sources are combined into polygons to create the geometry’s shape. Creating a custom geometry requires at least one element. If the `elements` array contains multiple objects, their order determines the arrangement of the geometry’s materials—for details, see the discussion of the materials property.

