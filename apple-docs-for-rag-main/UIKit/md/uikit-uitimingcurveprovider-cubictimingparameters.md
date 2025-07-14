

- UIKit
- UITimingCurveProvider
-  cubicTimingParameters 

Instance Property

# cubicTimingParameters

The cubic timing parameters to use.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var cubicTimingParameters: UICubicTimingParameters? { get }
```

**Required**

## Discussion

Implement this property and use it to provide your custom cubic timing information. If the value of the timingCurveType property is UITimingCurveType.builtin, UITimingCurveType.cubic, or UITimingCurveType.composed, you must return an object from this property. The object you return can specify one of the built-in UIKit curves, such as UIView.AnimationCurve.linear, or it can specify a timing curve based on a custom Bézier path.

For more information about configuring this object, see UICubicTimingParameters.

## See Also

### Getting the timing information

var timingCurveType: UITimingCurveType

The type of timing information to use.

**Required**

var springTimingParameters: UISpringTimingParameters?

The spring-based timing parameters to use.

**Required**

