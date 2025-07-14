

- UIKit
- UITimingCurveProvider
-  springTimingParameters 

Instance Property

# springTimingParameters

The spring-based timing parameters to use.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var springTimingParameters: UISpringTimingParameters? { get }
```

**Required**

## Discussion

Implement this property and use it to provide spring-based timing information. If the value of the timingCurveType property is UITimingCurveType.spring or UITimingCurveType.composed, you must return an object from this property.

For more information about configuring spring-based timing parameters, see UISpringTimingParameters.

## See Also

### Getting the timing information

var timingCurveType: UITimingCurveType

The type of timing information to use.

**Required**

var cubicTimingParameters: UICubicTimingParameters?

The cubic timing parameters to use.

**Required**

