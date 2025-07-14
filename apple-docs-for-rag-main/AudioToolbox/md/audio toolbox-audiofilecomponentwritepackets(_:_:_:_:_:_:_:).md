

- Audio Toolbox
-  AudioFileComponentWritePackets(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentWritePackets(\_:\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentWritePackets(
    _ inComponent: AudioFileComponent,
    _ inUseCache: Bool,
    _ inNumBytes: UInt32,
    _ inPacketDescriptions: UnsafePointer?,
    _ inStartingPacket: Int64,
    _ ioNumPackets: UnsafeMutablePointer,
    _ inBuffer: UnsafeRawPointer
) -> OSStatus
```

## See Also

### Reading and Writing Data

func AudioFileComponentReadBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPacketData(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPackets(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentWriteBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentReadBytesProc

typealias AudioFileComponentReadPacketDataProc

typealias AudioFileComponentReadPacketsProc

typealias AudioFileComponentWriteBytesProc

typealias AudioFileComponentWritePacketsProc

