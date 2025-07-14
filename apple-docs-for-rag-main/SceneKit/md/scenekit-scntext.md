

- SceneKit
-  SCNText 

Class

# SCNText

A geometry based on a string of text, optionally extruded to create a three-dimensional object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNText
```

## Overview

You provide text for the geometry using an NSString or NSAttributedString object. In the former case, the properties of the SCNText object determine the style and formatting of the entire body of text. When you create a text geometry from an attributed string, SceneKit styles the text according to the attributes in the string, and the properties of the SCNText object determine the default style for portions of the string that have no style attributes. SceneKit can create text geometry using any font and style supported by the Core Text framework, with the exception of bitmap fonts (such as those that define color emoji characters).

In the local coordinate system of the text geometry, the origin corresponds to the lower left corner of the text, with the text extending in the x- and y-axis dimensions. The geometry is centered along its z-axis. For example, if its extrusionDepth property is `1.0`, the geometry extends from `-0.5` to `0.5` along the z-axis. An extrusion depth of zero creates a flat, one-sided shape—the geometry is confined to the plane whose z-coordinate is `0.0`, and viewable only from its front unless its material’s isDoubleSided property is true.

To position and orient a text geometry in a scene, attach it to the geometry property of an SCNNode object.

Note

SceneKit creates geometry from text in a local coordinate system where one unit is one typographic point. For example, a text geometry whose font is Helvetica 36 (the default) may be up to 36 units tall. If your scene is arranged on a different scale, use the scale property of the node containing the text geometry to make it fit within your scene.

SceneKit can optionally *chamfer* an extruded text geometry by applying a cross-sectional contour to its extruded depth. You use the chamferRadius property to add a chamfer to the extruded text, and the chamferProfile property to control the shape of the chamfer.

A text geometry may contain one, three, or five geometry elements:

- If its extrusionDepth property is `0.0`, the text geometry has one element corresponding to its one visible side.

- If its extrusion depth is greater than zero and its chamferRadius property is `0.0`, the text geometry has three elements, corresponding to its front, back, and extruded sides.

- If both extrusion depth and chamfer radius are greater than zero, the text geometry has five elements, corresponding to its front, back, extruded sides, front chamfer, and back chamfer.

SceneKit can render each element using a different material. For details, see the description of the materials property in SCNGeometry.

## Topics

### Creating a Text Geometry

convenience init(string: Any?, extrusionDepth: CGFloat)

Creates a text geometry from a specified string, extruded with a specified depth.

### Managing the Geometry’s Text Content

var string: Any?

The string object whose text the geometry represents.

var font: UIFont!

The font that SceneKit uses to create geometry from the text.

### Managing Text Layout

var containerFrame: CGRect

A rectangle specifying the area in which SceneKit should lay out the text.

var isWrapped: Bool

A Boolean value that specifies whether SceneKit wraps long lines of text.

var alignmentMode: String

A constant that specifies how SceneKit horizontally aligns each line of text within its container.

var truncationMode: String

A constant that specifies how SceneKit truncates text that is too long to fit its container.

var textSize: CGSize

The two-dimensional extent of the text after layout.

### Managing the Text’s 3D Representation

var flatness: CGFloat

A number that determines the accuracy or smoothness of the text geometry.

var extrusionDepth: CGFloat

The extent of the extruded text in the z-axis direction. Animatable.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

## Relationships

### Inherits From

- SCNGeometry

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
- SCNAnimatable
- SCNBoundingVolume
- SCNShadable

## See Also

### Parametric Geometry

class SCNShape

A geometry based on a two-dimensional path, optionally extruded to create a three-dimensional object.

