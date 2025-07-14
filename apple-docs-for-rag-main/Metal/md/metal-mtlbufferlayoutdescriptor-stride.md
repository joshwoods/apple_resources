

- Metal
- MTLBufferLayoutDescriptor
-  stride 

Instance Property

# stride

The number of bytes from one buffer entry to the next.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var stride: Int { get set }
```

## Discussion

The default value is `1`. See Metal feature set tables (PDF) for `stride` alignment restrictions on GPU architectures.

## See Also

### Describing Fetch Behavior

var stepFunction: MTLStepFunction

Determines how and when compute functions fetch data.

var stepRate: Int

How frequently the step function should load data.

enum MTLStepFunction

The frequency and locations at which a function fetches attribute data.

