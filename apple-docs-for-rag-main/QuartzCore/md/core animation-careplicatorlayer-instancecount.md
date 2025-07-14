

- Core Animation
- CAReplicatorLayer
-  instanceCount 

Instance Property

# instanceCount

The number of copies to create, including the source layers.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var instanceCount: Int { get set }
```

## Discussion

Default value is `1`, no extra copies are created.

## See Also

### Related Documentation

Core Animation Programming Guide

### Setting Instance Display Properties

var instanceDelay: CFTimeInterval

Specifies the delay, in seconds, between replicated copies. Animatable.

var instanceTransform: CATransform3D

The transform matrix applied to the previous instance to produce the current instance. Animatable.

