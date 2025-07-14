

- Core Animation
- CAPropertyAnimation
-  isCumulative 

Instance Property

# isCumulative

Determines if the value of the property is the value at the end of the previous repeat cycle, plus the value of the current repeat cycle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var isCumulative: Bool { get set }
```

## Discussion

If true, then the value of the property is the value at the end of the previous repeat cycle, plus the value of the current repeat cycle. If false, the value of the property is simply the value calculated for the current repeat cycle. The default is false.

## See Also

### Property Value Calculation Behavior

var isAdditive: Bool

Determines if the value specified by the animation is added to the current render tree value to produce the new render tree value.

var valueFunction: CAValueFunction?

An optional value function that is applied to interpolated values.

