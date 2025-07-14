

- Core Animation
- CAAnimationGroup
-  animations 

Instance Property

# animations

An array of `CAAnimation` objects to be evaluated in the time space of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var animations: [CAAnimation]? { get set }
```

## Discussion

The animations run concurrently in the receiver’s time space.

## See Also

### Related Documentation

Core Animation Programming Guide

