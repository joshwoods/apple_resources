

- Core Animation
- CAValueFunctionName
-  translate 

Type Property

# translate

A value function that translates by the input values along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) translate values.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let translate: CAValueFunctionName
```

## See Also

### Constants

static let translateX: CAValueFunctionName

A value function translates by the input value along the x-axis. Animations referencing this value function must provide a single input value.

static let translateY: CAValueFunctionName

A value function translates by the input value along the y-axis. Animations referencing this value function must provide a single input value.

static let translateZ: CAValueFunctionName

A value function translates by the input value along the z-axis. Animations referencing this value function must provide a single input value.

