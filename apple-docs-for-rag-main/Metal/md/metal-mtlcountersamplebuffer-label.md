

- Metal
- MTLCounterSampleBuffer
-  label 

Instance Property

# label

A string that identifies the counter sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var label: String { get }
```

**Required**

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Inspecting the Counter Sample Buffer’s Configuration

var device: any MTLDevice

The GPU device instance that owns the counter sample buffer.

**Required**

var sampleCount: Int

The number of samples in the buffer.

**Required**

