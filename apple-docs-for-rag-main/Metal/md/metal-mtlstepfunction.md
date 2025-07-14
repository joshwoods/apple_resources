

- Metal
-  MTLStepFunction 

Enumeration

# MTLStepFunction

The frequency and locations at which a function fetches attribute data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
enum MTLStepFunction
```

## Topics

### Step options

case constant

The function fetches attribute data once.

case perInstance

The function fetches data based on the instance index.

case perPatch

The post-tessellation function fetches data based on the patch index of the patch.

case perPatchControlPoint

The post-tessellation function fetches data based on the control-point indices associated with the patch.

case perVertex

The vertex function fetches data for every vertex.

case threadPositionInGridX

The compute function fetches data based on the thread’s `x` coordinate.

case threadPositionInGridY

The compute function fetches data based on the thread’s `y` coordinate.

case threadPositionInGridXIndexed

The compute function fetches data by using the thread’s `x` coordinate to look up a value in the index buffer.

case threadPositionInGridYIndexed

The compute function fetches data by using the thread’s `y` coordinate to look up a value in the index buffer.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing Fetch Behavior

var stride: Int

The number of bytes from one buffer entry to the next.

var stepFunction: MTLStepFunction

Determines how and when compute functions fetch data.

var stepRate: Int

How frequently the step function should load data.

