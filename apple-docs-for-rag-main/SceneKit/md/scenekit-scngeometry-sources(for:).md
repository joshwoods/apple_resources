

- SceneKit
- SCNGeometry
-  sources(for:) 

Instance Method

# sources(for:)

Returns the geometry sources for a specified semantic.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func sources(for semantic: SCNGeometrySource.Semantic) -> [SCNGeometrySource]
```

## Parameters 

`semantic`  

A constant identifying a semantic for which to return geometry sources. See Geometry Semantic Identifiers for possible values.

## Return Value

An array of SCNGeometrySource objects, or `nil` if the geometry has no source for the specified semantic.

## Discussion

Each SCNGeometrySource object describes an attribute of all vertices in the geometry (such as vertex position, surface normal vector, color, or texture mapping coordinates) identified by the source’s semantic property. A geometry always has at least one source, for the vertex semantic, typically has additional sources for use in lighting and shading, and may have other sources for skeletal animation or surface subdivision information.

The vertex, normal, and color semantics each refer to at most one source. A geometry may have multiple sources for the texcoord semantic—in this case, indices in the returned array correspond to values for the mappingChannel property used when attaching textures to materials.

## See Also

### Related Documentation

convenience init(sources: [SCNGeometrySource], elements: [SCNGeometryElement]?)

Creates a new geometry built from the specified geometry sources and elements.

### Managing Geometry Data

var elements: [SCNGeometryElement]

An array of geometry elements that describe the geometry’s shape.

var sources: [SCNGeometrySource]

An array of geometry sources that provide vertex data for the geometry.

var elementCount: Int

The number of geometry elements in the geometry.

func element(at: Int) -> SCNGeometryElement

Returns the geometry element at a specified index.

