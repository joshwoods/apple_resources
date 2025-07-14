

- SceneKit
- SCNGeometry
-  elementCount 

Instance Property

# elementCount

The number of geometry elements in the geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var elementCount: Int { get }
```

## Discussion

Each SCNGeometryElement object describes how vertices from the geometry’s sources are combined into polygons to create the geometry’s shape. Visible geometries contain at least one element.

For geometries with multiple elements, you can use the materials property to attach different materials to each element.

## See Also

### Managing Geometry Data

var elements: [SCNGeometryElement]

An array of geometry elements that describe the geometry’s shape.

var sources: [SCNGeometrySource]

An array of geometry sources that provide vertex data for the geometry.

func element(at: Int) -> SCNGeometryElement

Returns the geometry element at a specified index.

func sources(for: SCNGeometrySource.Semantic) -> [SCNGeometrySource]

Returns the geometry sources for a specified semantic.

