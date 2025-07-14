

- Audio Toolbox
-  CopyInstrumentInfoFromSoundBank(\_:\_:) 

Function

# CopyInstrumentInfoFromSoundBank(\_:\_:)

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func CopyInstrumentInfoFromSoundBank(
    _ inURL: CFURL,
    _ outInstrumentInfo: UnsafeMutablePointer?>
) -> OSStatus
```

## See Also

### Instrument Functions

func CopyNameFromSoundBank(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Copies the name of a sound bank from a sound bank file at a specified URL.

var kInstrumentInfoKey_LSB: String

var kInstrumentInfoKey_MSB: String

var kInstrumentInfoKey_Name: String

var kInstrumentInfoKey_Program: String

