

- Metal
- MTLBufferLayoutDescriptor
-  stepRate 

Instance Property

# stepRate

How frequently the step function should load data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var stepRate: Int { get set }
```

## Discussion

The interpretation of this value depends on the setting of `stepFunction`.

## See Also

### Describing Fetch Behavior

var stride: Int

The number of bytes from one buffer entry to the next.

var stepFunction: MTLStepFunction

Determines how and when compute functions fetch data.

enum MTLStepFunction

The frequency and locations at which a function fetches attribute data.

