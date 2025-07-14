

- Core Audio Types
- AudioBuffer
-  mNumberChannels 

Instance Property

# mNumberChannels

The number of interleaved channels in the buffer.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mNumberChannels: UInt32
```

## Discussion

A value of `1` indicates the buffer is noninterleaved.

## See Also

### Accessing the Audio

var mDataByteSize: UInt32

The number of bytes in the buffer.

var mData: UnsafeMutableRawPointer?

A pointer to a buffer of audio data.

