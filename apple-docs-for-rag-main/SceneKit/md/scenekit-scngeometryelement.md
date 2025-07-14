

- SceneKit
-  SCNGeometryElement 

Class

# SCNGeometryElement

A container for index data describing how vertices connect to define a three-dimensional object, or geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNGeometryElement
```

## Overview

You use geometry elements together with SCNGeometrySource objects to define custom SCNGeometry objects or to inspect the data that composes an existing geometry. You create a custom geometry using a three-step process:

1.  Create one or more SCNGeometrySource objects, each of which defines per-vertex information such as position, surface normal, or texture coordinates for all vertices in the geometry.

2.  Create at least one SCNGeometryElement object, containing an array of indices identifying vertices in the geometry sources and describing the drawing primitive that SceneKit uses to connect the vertices when rendering the geometry.

3.  Create an SCNGeometry instance from the geometry sources and geometry elements.

When SceneKit renders a geometry, each geometry element corresponds to a drawing command sent to the GPU. Because different rendering states require separate drawing commands, you can define a geometry using multiple geometry elements. For example, the teapot geometry shown below has four geometry elements, so you can assign up to four SCNMaterial objects in order to render each element with a different appearance. But because each drawing command incurs a CPU time overhead when rendering, minimizing the number of elements in a custom geometry can improve rendering performance.

## Topics

### Creating a Geometry Element

convenience init&lt;IndexType>(indices: [IndexType], primitiveType: SCNGeometryPrimitiveType)

Creates a geometry element from the specified array of index values.

convenience init(data: Data?, primitiveType: SCNGeometryPrimitiveType, primitiveCount: Int, bytesPerIndex: Int)

Creates a geometry element from the specified data and options.

### Working with Indexes

var data: Data

The data describing the geometry element.

var bytesPerIndex: Int

The number of bytes that represent each index value in the element’s data.

var primitiveType: SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering the geometry element.

enum SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

var primitiveCount: Int

The number of primitives in the element.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

### Rendering Point Clouds

Use these properties to display a geometry as a collection of points, rather than as a solid surface or wireframe.

var pointSize: CGFloat

The width of each point in the geometry element, as measured in the geometry’s local 3D coordinate space.

var minimumPointScreenSpaceRadius: CGFloat

The smallest radius, measured in screen points, at which to render any point in the geometry element.

var maximumPointScreenSpaceRadius: CGFloat

The largest radius, measured in screen points, at which to render any point in the geometry element.

### Initializers

convenience init(buffer: any MTLBuffer, primitiveType: SCNGeometryPrimitiveType, primitiveCount: Int, bytesPerIndex: Int)

convenience init(buffer: any MTLBuffer, primitiveType: SCNGeometryPrimitiveType, primitiveCount: Int, indicesChannelCount: Int, interleavedIndicesChannels: Bool, bytesPerIndex: Int)

convenience init(data: Data?, primitiveType: SCNGeometryPrimitiveType, primitiveCount: Int, indicesChannelCount: Int, interleavedIndicesChannels: Bool, bytesPerIndex: Int)

### Instance Properties

var hasInterleavedIndicesChannels: Bool

var indicesChannelCount: Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Geometry

class SCNGeometry

A three-dimensional shape (also called a model or mesh) that can be displayed in a scene, with attached materials that define its appearance.

class SCNGeometrySource

A container for vertex data forming part of the definition for a three-dimensional object, or geometry.

Built-in Geometry Types

Basic shapes—such as spheres, boxes, and planes—and features for generating 3D objects from 2D text and Bézier curves.

