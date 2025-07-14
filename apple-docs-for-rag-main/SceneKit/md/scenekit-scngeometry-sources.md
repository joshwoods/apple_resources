

- SceneKit
- SCNGeometry
-  sources 

Instance Property

# sources

An array of geometry sources that provide vertex data for the geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var sources: [SCNGeometrySource] { get }
```

## Discussion

Each SCNGeometrySource object describes an attribute of all vertices in the geometry (such as vertex position, surface normal vector, color, or texture mapping coordinates) identified by the source’s semantic property. A geometry always has at least one source (for the vertex semantic), typically has additional sources for use in lighting and shading, and may have other sources for skeletal animation or surface subdivision information.

## See Also

### Managing Geometry Data

var elements: [SCNGeometryElement]

An array of geometry elements that describe the geometry’s shape.

var elementCount: Int

The number of geometry elements in the geometry.

func element(at: Int) -> SCNGeometryElement

Returns the geometry element at a specified index.

func sources(for: SCNGeometrySource.Semantic) -> [SCNGeometrySource]

Returns the geometry sources for a specified semantic.

