

- Audio Toolbox
-  AudioConverterNewWithOptions(\_:\_:\_:\_:) 

Function

# AudioConverterNewWithOptions(\_:\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func AudioConverterNewWithOptions(
    _ inSourceFormat: UnsafePointer,
    _ inDestinationFormat: UnsafePointer,
    _ inOptions: AudioConverterOptions,
    _ outAudioConverter: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Functions

func AudioComponentValidateWithResults(AudioComponent, CFDictionary?, (AudioComponentValidationResult, CFDictionary) -> Void) -> OSStatus

func AudioConverterPrepare(UInt32, UnsafeMutableRawPointer?, ((OSStatus) -> Void)?)

func AudioFileComponentGetUserDataAtOffset(AudioFileComponent, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetUserDataSize64(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

