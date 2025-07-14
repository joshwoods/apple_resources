

- SceneKit
- SCNHitTestResult
-  textureCoordinates(withMappingChannel:) 

Instance Method

# textureCoordinates(withMappingChannel:)

Returns the texture coordinates at the point of intersection for the specified texture mapping channel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func textureCoordinates(withMappingChannel channel: Int) -> CGPoint
```

## Parameters 

`channel`  

The index of the mapping channel in which to look up texture coordinates.

## Return Value

The texture coordinates at the point of intersection, or CGPointZero if the geometry does not have a texture coordinate source for the specified channel.

## Discussion

An SCNGeometry object can contain multiple sources of texture coordinates, or texture mapping channels. (With multiple channels, you can map texture images for different material properties in different ways.) To use the texture coordinates of a hit-test result, specify which texture coordinate source to look up coordinates in.

For example, to add “scorch marks” to a game character hit by a laser, you might modify a texture image mapped to the multiply property of the geometry’s material. Use the mappingChannel index from that material property as the `channel` parameter when calling textureCoordinates(withMappingChannel:) to ensure that you modify the correct location in the texture image.

## See Also

### Retrieving Information About a Hit-Test Result

var node: SCNNode

The node whose geometry intersects the search ray.

var geometryIndex: Int

The index of the geometry element whose surface the search ray intersects.

var faceIndex: Int

The index of the primitive in the geometry element intersected by the search ray.

var localCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the local coordinate system of the node containing the geometry.

var worldCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the scene’s world coordinate system.

var localNormal: SCNVector3

The surface normal vector at the point of intersection, in the local coordinate system of the node containing the geometry intersected by the search ray.

var worldNormal: SCNVector3

The surface normal vector at the point of intersection, in the scene’s world coordinate system.

var modelTransform: SCNMatrix4

The world transform matrix of the node containing the intersection.

