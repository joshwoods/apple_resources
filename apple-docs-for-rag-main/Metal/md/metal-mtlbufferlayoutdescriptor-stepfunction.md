

- Metal
- MTLBufferLayoutDescriptor
-  stepFunction 

Instance Property

# stepFunction

Determines how and when compute functions fetch data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var stepFunction: MTLStepFunction { get set }
```

## See Also

### Describing Fetch Behavior

var stride: Int

The number of bytes from one buffer entry to the next.

var stepRate: Int

How frequently the step function should load data.

enum MTLStepFunction

The frequency and locations at which a function fetches attribute data.

