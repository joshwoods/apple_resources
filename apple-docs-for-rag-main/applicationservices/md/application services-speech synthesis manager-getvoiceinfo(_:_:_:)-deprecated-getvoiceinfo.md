

- Application Services
- Speech Synthesis Manager
-  GetVoiceInfo(\_:\_:\_:) Deprecated

Function

# GetVoiceInfo(\_:\_:\_:)

Gets the same information about a voice that the `GetVoiceDescription` function provides,or to determine in which file and resource a voice is stored.

macOS 10.0–13.0Deprecated

``` source
func GetVoiceInfo(
    _ voice: UnsafePointer?,
    _ selector: OSType,
    _ voiceInfo: UnsafeMutableRawPointer
) -> OSErr
```

## Parameters 

`voice`  

A pointer to the voice specification structure identifying the voice about which your application requires information, or `NULL` to obtain information on the system default voice.

`selector`  

A specification of the type of data being requested. For current versions of the Speech Synthesis Manager, you should set this field either to `soVoiceDescription`, if you would like to use the `GetVoiceInfo` function to mimic the `GetVoiceDescription` function, or to `soVoiceFile`, if you would like to obtain information about the location of a voice on disk.

`voiceInfo`  

A pointer to the appropriate data structure. If the selector is `soVoiceDescription`, then `voiceInfo` should be a pointer to a voice description structure, and the `length` field of the structure should be set to the length of the voice description structure. If the selector is `soVoiceFile`, then `voiceInfo` should be a pointer to a voice file information structure.

## Return Value

A resultcode. See Result Codes.

## Discussion

This function is intended primarily for use by synthesizers,but an application can call it too.

The `GetVoiceInfo` functionaccepts a selector in the `selector` parameterthat determines the type of information you wish to obtain aboutthe voice specified in the `voice` parameter. Thefunction then fills the fields of the data structure appropriateto the selector you specify in the `voiceInfo` parameter.

If the voice specification is invalid, `GetVoiceInfo` returnsa `voiceNotFound` error.If there is not enough memory to load the voice into memory to obtaininformation about it, `GetVoiceInfo` returnsthe result code `memFullErr`.

## See Also

### Getting Information About Voices

func CountVoices(UnsafeMutablePointer&lt;Int16>) -> OSErr

Determines how many voices are available.

Deprecated

func GetIndVoice(Int16, UnsafeMutablePointer&lt;VoiceSpec>) -> OSErr

Gets a voice specification structure for a voice bypassing an index to the `GetIndVoice` function.

Deprecated

func GetVoiceDescription(UnsafePointer&lt;VoiceSpec>?, UnsafeMutablePointer&lt;VoiceDescription>?, Int) -> OSErr

Gets a description of a voice by using the `GetVoiceDescription` function.

Deprecated

func MakeVoiceSpec(OSType, OSType, UnsafeMutablePointer&lt;VoiceSpec>) -> OSErr

Sets the fields of a voice specification structure.

Deprecated

