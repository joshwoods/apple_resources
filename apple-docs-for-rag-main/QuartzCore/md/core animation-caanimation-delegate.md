

- Core Animation
- CAAnimation
-  delegate 

Instance Property

# delegate

Specifies the receiver’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var delegate: (any CAAnimationDelegate)? { get set }
```

## Discussion

Defaults to `nil`.

Important

The `delegate` object is retained by the receiver. This is a rare exception to the memory management rules described in Advanced Memory Management Programming Guide.

An instance of `CAAnimation` should not be set as a delegate of itself. Doing so (outside of a garbage-collected environment) will cause retain cycles.

