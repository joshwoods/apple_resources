

- Audio Toolbox
-  AudioFileComponentGetUserDataSize64(\_:\_:\_:\_:) 

Function

# AudioFileComponentGetUserDataSize64(\_:\_:\_:\_:)

macOS 14.0+

``` source
func AudioFileComponentGetUserDataSize64(
    _ inComponent: AudioFileComponent,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ outUserDataSize: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Functions

func AudioComponentValidateWithResults(AudioComponent, CFDictionary?, (AudioComponentValidationResult, CFDictionary) -> Void) -> OSStatus

func AudioConverterNewWithOptions(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, AudioConverterOptions, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

func AudioConverterPrepare(UInt32, UnsafeMutableRawPointer?, ((OSStatus) -> Void)?)

func AudioFileComponentGetUserDataAtOffset(AudioFileComponent, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

