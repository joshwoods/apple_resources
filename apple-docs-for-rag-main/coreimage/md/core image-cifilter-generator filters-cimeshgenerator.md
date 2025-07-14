

- Core Image
- CIFilter
- Generator Filters
-  CIMeshGenerator 

Protocol

# CIMeshGenerator

The properties you use to configure a mesh generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMeshGenerator
```

## Topics

### Instance Properties

var color: CIColor

The color of the rendered mesh.

**Required**

var mesh: [Any]

An array that describes the mesh to render.

**Required**

var width: Float

The width of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func meshGenerator() -> any CIFilter &amp; CIMeshGenerator

Generates a pattern made from an array of line segments.

