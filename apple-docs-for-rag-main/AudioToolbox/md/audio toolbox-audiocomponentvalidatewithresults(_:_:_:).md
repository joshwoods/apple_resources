

- Audio Toolbox
-  AudioComponentValidateWithResults(\_:\_:\_:) 

Function

# AudioComponentValidateWithResults(\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func AudioComponentValidateWithResults(
    _ inComponent: AudioComponent,
    _ inValidationParameters: CFDictionary?,
    _ inCompletionHandler: @escaping (AudioComponentValidationResult, CFDictionary) -> Void
) -> OSStatus
```

## See Also

### Functions

func AudioConverterNewWithOptions(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, AudioConverterOptions, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

func AudioConverterPrepare(UInt32, UnsafeMutableRawPointer?, ((OSStatus) -> Void)?)

func AudioFileComponentGetUserDataAtOffset(AudioFileComponent, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetUserDataSize64(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

