

- Core Animation
- CAMediaTiming
-  repeatDuration 

Instance Property

# repeatDuration

Determines how many seconds the animation will repeat for.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var repeatDuration: CFTimeInterval { get set }
```

**Required**

## Discussion

Defaults to 0. If the `repeatDuration` is 0, it is ignored. If both repeatDuration and repeatCount are specified the behavior is undefined.

## See Also

### Repeating Animations

var repeatCount: Float

Determines the number of times the animation will repeat.

**Required**

