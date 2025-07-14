

- UIKit
- UITimingCurveType
-  UITimingCurveType.composed 

Case

# UITimingCurveType.composed

Use a combination of timing parameters. This type of curve starts with the curve defined by the cubicTimingParameters property and modifies it using the spring information in the springTimingParameters property.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
case composed
```

## See Also

### Constants

case builtin

Use the built-in UIKit timing curves. Specify this value when you want to use one of the constants in the UIView.AnimationCurve type. Specify the desired curve using the cubicTimingParameters property.

case cubic

Use a custom cubic Bézier curve. Specify the curve information using the cubicTimingParameters property.

case spring

Use a custom spring animation. Specify the desired curve using the springTimingParameters property.

