

- UIKit
- UITimingCurveProvider
-  timingCurveType 

Instance Property

# timingCurveType

The type of timing information to use.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var timingCurveType: UITimingCurveType { get }
```

**Required**

## Discussion

Use this property to specify the type of timing information your timing curve object supplies. The value of this property determines whether the view property animator uses the object in the cubicTimingParameters or springTimingParameters property for timing information.

## See Also

### Getting the timing information

var cubicTimingParameters: UICubicTimingParameters?

The cubic timing parameters to use.

**Required**

var springTimingParameters: UISpringTimingParameters?

The spring-based timing parameters to use.

**Required**

