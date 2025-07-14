

- Metal
- MTLPrimitiveAccelerationStructureDescriptor
-  geometryDescriptors 

Instance Property

# geometryDescriptors

An array that contains the individual pieces of geometry that compose the acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var geometryDescriptors: [MTLAccelerationStructureGeometryDescriptor]? { get set }
```

## Discussion

The value of the motionKeyframeCount property determines what kinds of geometry descriptors you can assign to this property and how you need to configure them.

If the value of motionKeyframeCount is greater than 1, then the geometry descriptors must be either MTLAccelerationStructureMotionBoundingBoxGeometryDescriptor or MTLAccelerationStructureMotionTriangleGeometryDescriptor objects. Further, you must provide exactly that many keyframes of data when creating those geometry descriptors. If motionKeyframeCount is 1, use MTLAccelerationStructureBoundingBoxGeometryDescriptor or MTLAccelerationStructureTriangleGeometryDescriptor objects instead.

## See Also

### Related Documentation

var motionKeyframeCount: Int

The number of keyframes in the geometry data.

