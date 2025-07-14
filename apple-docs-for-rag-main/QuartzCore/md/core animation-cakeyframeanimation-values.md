

- Core Animation
- CAKeyframeAnimation
-  values 

Instance Property

# values

An array of objects that specify the keyframe values to use for the animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var values: [Any]? { get set }
```

## Discussion

The keyframe values represent the values through which the animation must proceed. The time at which a given keyframe value is applied to the layer depends on the animation timing, which is controlled by the calculationMode, keyTimes, and timingFunctions properties. Values between keyframes are created using interpolation, unless the calculation mode is set to discrete.

Depending on the type of the property, you may need to wrap the values in this array with an NSNumber of NSValue object. For some Core Graphics data types, you may also need to cast them to `id` before adding them to the array.

The values in this property are used only if the value in the path property is `nil`.

## See Also

### Related Documentation

Core Animation Programming Guide

### Providing keyframe values

var path: CGPath?

The path for a point-based property to follow.

