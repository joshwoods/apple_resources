

- Core Animation
- CATransition
-  endProgress 

Instance Property

# endProgress

Indicates the end point of the receiver as a fraction of the entire transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var endProgress: Float { get set }
```

## Discussion

The value must be greater than or equal to startProgress, and not greater than 1.0. If `endProgress` is less than startProgress the behavior is undefined. The default value is 1.0.

## See Also

### Transition start and end point

var startProgress: Float

Indicates the start point of the receiver as a fraction of the entire transition.

