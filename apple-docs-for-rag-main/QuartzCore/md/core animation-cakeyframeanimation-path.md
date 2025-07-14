

- Core Animation
- CAKeyframeAnimation
-  path 

Instance Property

# path

The path for a point-based property to follow.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var path: CGPath? { get set }
```

## Discussion

For layer properties that contain a CGPoint data type, the path object you assign to this property defines the values for that property over the length of the animation. If you specify a value for this property, any data in the values property is ignored.

Any timing values you specify for the animation are applied to the points used to create the path. Paths can contain points defining move-to, line-to, or curve-to segments. The end point of a line-to or curve-to segment defines the keyframe value. All other points between that end value and the previous value are then interpolated. Move-to segments do not define separate keyframe values.

How the animation proceeds along the path is dependent on the value in the calculationMode property. To achieve a smooth, constant velocity animation along the path, set the calculationMode property to paced or cubicPaced. To create an animation where the location value jumps from keyframe point to keyframe point (without interpolation in between), use the discrete value. To animate along the path by interpolating values between points, use the linear value.

## See Also

### Related Documentation

var rotationMode: CAAnimationRotationMode?

Determines whether objects animating along the path rotate to match the path tangent.

### Providing keyframe values

var values: [Any]?

An array of objects that specify the keyframe values to use for the animation.

