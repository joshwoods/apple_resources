

- Audio Toolbox
-  AudioFileComponentWritePacketsProc 

Type Alias

# AudioFileComponentWritePacketsProc

macOS

``` source
typealias AudioFileComponentWritePacketsProc = (UnsafeMutableRawPointer, DarwinBoolean, UInt32, UnsafePointer?, Int64, UnsafeMutablePointer, UnsafeRawPointer) -> OSStatus
```

## See Also

### Reading and Writing Data

func AudioFileComponentReadBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPacketData(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPackets(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentWriteBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

func AudioFileComponentWritePackets(AudioFileComponent, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentReadBytesProc

typealias AudioFileComponentReadPacketDataProc

typealias AudioFileComponentReadPacketsProc

typealias AudioFileComponentWriteBytesProc

