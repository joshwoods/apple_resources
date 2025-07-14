

- SceneKit
-  SCNLevelOfDetail 

Class

# SCNLevelOfDetail

An alternate resolution for a geometry that SceneKit automatically substitutes to improve rendering performance.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNLevelOfDetail
```

## Overview

You use level-of-detail objects when you have a detailed geometry that appears at several apparent sizes in a scene. For example, the teapot model on the the left in the figure below has 256 polygons, the model at center has 1024 polygons, and the model on the right has 14,400 polygons. If all three models appear close to the camera, filling most of the rendered view, the difference in detail between them is clearly visible—but if they appear far away, taking up a small area of the view, the difference is much less obvious. Rendering higher-resolution geometries incurs a higher performance cost.

When you associate one or more level-of-detail objects with a SCNGeometry object using its levelsOfDetail property, SceneKit automatically substitutes alternate geometries when appropriate. For example, the two lower-resolution teapot models seen above can be added as levels of detail for the high-resolution model.

For each level of detail, you specify either a world-space distance or a screen-space radius. The measure you specify determines the threshold where SceneKit automatically renders that level of detail’s alternate geometry instead of the original geometry. If you specify a distance, the alternate geometry appears when the node containing the geometry is moved that distance away from the camera. If you specify a radius, the alternate geometry appears when the pixel area covered by the rendered geometry is smaller than a circle of that radius.

The geometries associated with lower levels of detail need not share all attributes of the original geometry. For example, you can use different materials for levels of detail that only appear when far away from the camera, disabling expensive features such as per-pixel lighting, reflection mapping, or custom shader programs.

## Topics

### Creating a Level of Detail

convenience init(geometry: SCNGeometry?, screenSpaceRadius: CGFloat)

Creates a level of detail with the specified geometry and threshold pixel radius.

convenience init(geometry: SCNGeometry?, worldSpaceDistance: CGFloat)

Creates a level of detail with the specified geometry and threshold camera distance.

### Inspecting a Level of Detail

var geometry: SCNGeometry?

The geometry associated with this level of detail.

var screenSpaceRadius: CGFloat

The maximum radius (in pixels) of the geometry’s bounding sphere for this level of detail to appear.

var worldSpaceDistance: CGFloat

The minimum distance from the current point of view for this level of detail to appear.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Optimizing Level of Detail

var levelsOfDetail: [SCNLevelOfDetail]?

An array of SCNLevelOfDetail objects for managing the geometry’s appearance when viewed from far away.

