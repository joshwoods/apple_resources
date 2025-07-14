

- Audio Toolbox
-  CopyNameFromSoundBank(\_:\_:) 

Function

# CopyNameFromSoundBank(\_:\_:)

Copies the name of a sound bank from a sound bank file at a specified URL.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CopyNameFromSoundBank(
    _ inURL: CFURL,
    _ outName: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`inURL`  

A URL that points to the sound bank whose name you want to get.

`outName`  

The name of the sound bank.

## Return Value

A result code.

## See Also

### Instrument Functions

func CopyInstrumentInfoFromSoundBank(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

var kInstrumentInfoKey_LSB: String

var kInstrumentInfoKey_MSB: String

var kInstrumentInfoKey_Name: String

var kInstrumentInfoKey_Program: String

