

- Audio Toolbox
-  AudioCodecAppendInputBufferList(\_:\_:\_:\_:\_:) 

Function

# AudioCodecAppendInputBufferList(\_:\_:\_:\_:\_:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecAppendInputBufferList(
    _ inCodec: AudioCodec,
    _ inBufferList: UnsafePointer,
    _ ioNumberPackets: UnsafeMutablePointer,
    _ inPacketDescription: UnsafePointer?,
    _ outBytesConsumed: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Configuring Buffers

func AudioCodecProduceOutputBufferList(AudioCodec, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

