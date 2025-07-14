

- Core Animation
- CAValueFunctionName
-  translateZ 

Type Property

# translateZ

A value function translates by the input value along the z-axis. Animations referencing this value function must provide a single input value.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let translateZ: CAValueFunctionName
```

## See Also

### Constants

static let translate: CAValueFunctionName

A value function that translates by the input values along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) translate values.

static let translateX: CAValueFunctionName

A value function translates by the input value along the x-axis. Animations referencing this value function must provide a single input value.

static let translateY: CAValueFunctionName

A value function translates by the input value along the y-axis. Animations referencing this value function must provide a single input value.

