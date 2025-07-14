

- Audio Toolbox
-  AudioFileComponentReadPacketDataProc 

Type Alias

# AudioFileComponentReadPacketDataProc

macOS

``` source
typealias AudioFileComponentReadPacketDataProc = (UnsafeMutableRawPointer, DarwinBoolean, UnsafeMutablePointer, UnsafeMutablePointer?, Int64, UnsafeMutablePointer, UnsafeMutableRawPointer) -> OSStatus
```

## See Also

### Reading and Writing Data

func AudioFileComponentReadBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPacketData(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPackets(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentWriteBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

func AudioFileComponentWritePackets(AudioFileComponent, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentReadBytesProc

typealias AudioFileComponentReadPacketsProc

typealias AudioFileComponentWriteBytesProc

typealias AudioFileComponentWritePacketsProc

