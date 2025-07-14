

- Audio Toolbox
-  AudioToolbox Functions 

API Collection

# AudioToolbox Functions

## Topics

### Functions

func AudioComponentValidateWithResults(AudioComponent, CFDictionary?, (AudioComponentValidationResult, CFDictionary) -> Void) -> OSStatus

func AudioConverterNewWithOptions(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, AudioConverterOptions, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

func AudioConverterPrepare(UInt32, UnsafeMutableRawPointer?, ((OSStatus) -> Void)?)

func AudioFileComponentGetUserDataAtOffset(AudioFileComponent, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetUserDataSize64(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

## See Also

### Reference

AudioToolbox Structures

AudioToolbox Enumerations

AudioToolbox Constants

AudioToolbox Data Types

