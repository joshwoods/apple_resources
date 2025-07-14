

- Core Animation
- CATransition
-  startProgress 

Instance Property

# startProgress

Indicates the start point of the receiver as a fraction of the entire transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var startProgress: Float { get set }
```

## Discussion

Legal values are numbers between 0.0 and 1.0. For example, to start the transition half way through its progress set `startProgress` to 0.5. The default value is 0.

## See Also

### Related Documentation

Core Animation Programming Guide

### Transition start and end point

var endProgress: Float

Indicates the end point of the receiver as a fraction of the entire transition.

