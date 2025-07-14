

- SceneKit
-  SCNBoundingVolume 

Protocol

# SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNBoundingVolume : NSObjectProtocol
```

## Overview

This protocol defines features adopted by both the SCNNode and SCNGeometry classes.

A bounding box is the smallest volume, in the shape of a rectangle aligned to the axes of the local coordinate space, that entirely contains an object. Scene Kit defines a bounding box using two points: a minimum and maximum corner. Similarly, a bounding sphere is the smallest sphere containing an object.

By default, Scene Kit automatically determines the minimal bounding volumes for geometries based on their vertex positions in model space. The bounding volume of a node with an attached geometry is the bounding volume of the geometry, expressed in the node’s local space. The bounding volume of a node containing child nodes is the minimal volume that encloses the bounding volumes of the node’s children.

Scene Kit uses the bounding volume of an object when determining how to render a scene. For example, an SCNCamera object uses the bounding boxes of visible elements in a scene to determine the its depth limits. You can override a bounding volume to change this behavior. For example, if a building model has a long, narrow antenna, the default bounding box includes that feature, so the default camera view for that model will be off-center with respect to the building itself. If you set a new bounding box that includes only the main part of the building, the default camera view will center on the building and ignore the antenna.

### Getting and Setting Bounding Volumes

Read the boundingBox or boundingSphere property, getBoundingBoxMin:max: or getBoundingSphereCenter:radius: methods in Objective-C, to retrieve information about an object’s bounding box or sphere. To override the automatically determined bounding volume of an object, set a new value for the boundingBox property, the setBoundingBoxMin:max: method in Objective-C.

## Topics

### Measuring an Object’s Bounding Volume

var boundingBox: (min: SCNVector3, max: SCNVector3)

The minimum and maximum corner points of the object’s bounding box.

var boundingSphere: (center: SCNVector3, radius: Float)

The center point and radius of the object’s bounding sphere.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNBox
- SCNCapsule
- SCNCone
- SCNCylinder
- SCNFloor
- SCNGeometry
- SCNNode
- SCNPlane
- SCNPyramid
- SCNReferenceNode
- SCNShape
- SCNSphere
- SCNText
- SCNTorus
- SCNTube

## See Also

### Managing Geometry Attributes

var name: String?

A name associated with the geometry object.

