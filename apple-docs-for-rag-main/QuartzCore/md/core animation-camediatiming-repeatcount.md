

- Core Animation
- CAMediaTiming
-  repeatCount 

Instance Property

# repeatCount

Determines the number of times the animation will repeat.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var repeatCount: Float { get set }
```

**Required**

## Discussion

May be fractional. If the `repeatCount` is 0, it is ignored. Defaults to 0. If both repeatDuration and repeatCount are specified the behavior is undefined.

Setting this property to greatestFiniteMagnitude will cause the animation to repeat forever.

## See Also

### Repeating Animations

var repeatDuration: CFTimeInterval

Determines how many seconds the animation will repeat for.

**Required**

