

- Audio Toolbox
-  AudioCodecProduceOutputBufferList(\_:\_:\_:\_:\_:) 

Function

# AudioCodecProduceOutputBufferList(\_:\_:\_:\_:\_:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecProduceOutputBufferList(
    _ inCodec: AudioCodec,
    _ ioBufferList: UnsafeMutablePointer,
    _ ioNumberPackets: UnsafeMutablePointer,
    _ outPacketDescription: UnsafeMutablePointer?,
    _ outStatus: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Configuring Buffers

func AudioCodecAppendInputBufferList(AudioCodec, UnsafePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;UInt32>, UnsafePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

