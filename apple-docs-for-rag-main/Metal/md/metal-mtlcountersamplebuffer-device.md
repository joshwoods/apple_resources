

- Metal
- MTLCounterSampleBuffer
-  device 

Instance Property

# device

The GPU device instance that owns the counter sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

You can store a GPU device’s counter set data only with a counter sample buffer that you create from the same device.

## See Also

### Inspecting the Counter Sample Buffer’s Configuration

var label: String

A string that identifies the counter sample buffer.

**Required**

var sampleCount: Int

The number of samples in the buffer.

**Required**

