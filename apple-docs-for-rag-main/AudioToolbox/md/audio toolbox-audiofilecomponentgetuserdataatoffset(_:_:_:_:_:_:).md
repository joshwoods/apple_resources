

- Audio Toolbox
-  AudioFileComponentGetUserDataAtOffset(\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentGetUserDataAtOffset(\_:\_:\_:\_:\_:\_:)

macOS 14.0+

``` source
func AudioFileComponentGetUserDataAtOffset(
    _ inComponent: AudioFileComponent,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ inOffset: Int64,
    _ ioUserDataSize: UnsafeMutablePointer,
    _ outUserData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Functions

func AudioComponentValidateWithResults(AudioComponent, CFDictionary?, (AudioComponentValidationResult, CFDictionary) -> Void) -> OSStatus

func AudioConverterNewWithOptions(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, AudioConverterOptions, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

func AudioConverterPrepare(UInt32, UnsafeMutableRawPointer?, ((OSStatus) -> Void)?)

func AudioFileComponentGetUserDataSize64(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

