

- Audio Toolbox
-  AudioFileComponentReadPacketData(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentReadPacketData(\_:\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentReadPacketData(
    _ inComponent: AudioFileComponent,
    _ inUseCache: Bool,
    _ ioNumBytes: UnsafeMutablePointer,
    _ outPacketDescriptions: UnsafeMutablePointer?,
    _ inStartingPacket: Int64,
    _ ioNumPackets: UnsafeMutablePointer,
    _ outBuffer: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Reading and Writing Data

func AudioFileComponentReadBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPackets(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentWriteBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

func AudioFileComponentWritePackets(AudioFileComponent, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentReadBytesProc

typealias AudioFileComponentReadPacketDataProc

typealias AudioFileComponentReadPacketsProc

typealias AudioFileComponentWriteBytesProc

typealias AudioFileComponentWritePacketsProc

