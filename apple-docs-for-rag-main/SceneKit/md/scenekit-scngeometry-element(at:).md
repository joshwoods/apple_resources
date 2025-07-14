

- SceneKit
- SCNGeometry
-  element(at:) 

Instance Method

# element(at:)

Returns the geometry element at a specified index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func element(at elementIndex: Int) -> SCNGeometryElement
```

## Parameters 

`elementIndex`  

The index of the geometry element.

## Return Value

A geometry element.

## Discussion

Each SCNGeometryElement object describes how vertices from the geometry’s sources are combined into polygons to create the geometry’s shape. Visible geometries contain at least one element.

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

func sources(for: SCNGeometrySource.Semantic) -> [SCNGeometrySource]

Returns the geometry sources for a specified semantic.

