

- Core Animation
- CAValueFunctionName
-  scaleZ 

Type Property

# scaleZ

A value function that scales by the input value along the z-axis. Animations referencing this value function must provide a single animation value.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let scaleZ: CAValueFunctionName
```

## See Also

### Constants

static let scale: CAValueFunctionName

A value function scales by the input value along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) scale values.

static let scaleX: CAValueFunctionName

A value function scales by the input value along the x-axis. Animations referencing this value transform function must provide a single animation value.

static let scaleY: CAValueFunctionName

A value function scales by the input value along the y-axis. Animations referencing this value function must provide a single animation value.

