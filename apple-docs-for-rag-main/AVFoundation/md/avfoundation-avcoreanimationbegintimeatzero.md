

- AVFoundation
-  AVCoreAnimationBeginTimeAtZero 

Global Variable

# AVCoreAnimationBeginTimeAtZero

A value that sets an animation begin time to `0`.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVCoreAnimationBeginTimeAtZero: CFTimeInterval
```

## Discussion

The constant is a small, non-zero, positive value which prevents CoreAnimation from replacing `0.0` with CACurrentMediaTime().

