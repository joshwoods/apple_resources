

- Audio Toolbox
-  AudioConverterPrepare(\_:\_:\_:) 

Function

# AudioConverterPrepare(\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func AudioConverterPrepare(
    _ inFlags: UInt32,
    _ ioReserved: UnsafeMutableRawPointer?,
    _ inCompletionBlock: ((OSStatus) -> Void)?
)
```

## See Also

### Functions

func AudioComponentValidateWithResults(AudioComponent, CFDictionary?, (AudioComponentValidationResult, CFDictionary) -> Void) -> OSStatus

func AudioConverterNewWithOptions(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, AudioConverterOptions, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

func AudioFileComponentGetUserDataAtOffset(AudioFileComponent, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetUserDataSize64(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

