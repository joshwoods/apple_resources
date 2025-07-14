

- Application Services
- Speech Synthesis Manager
-  MakeVoiceSpec(\_:\_:\_:) Deprecated

Function

# MakeVoiceSpec(\_:\_:\_:)

Sets the fields of a voice specification structure.

macOS 10.0–13.0Deprecated

``` source
func MakeVoiceSpec(
    _ creator: OSType,
    _ id: OSType,
    _ voice: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`creator`  

The ID of the synthesizer that your application requires.

`id`  

The ID of the voice on the synthesizer specified by the `creator` parameter.

`voice`  

A pointer to the voice specification structure whose fields are to be filled in.

## Return Value

A resultcode. See Result Codes.

## Discussion

A voice specification structure is a unique voice ID usedby the Speech Synthesis Manager. Most voice management functionsexpect to be passed a pointer to a voice specification structure.When you already know the creator and ID for a voice, you shoulduse the `MakeVoiceSpec` functionto create such a structure rather than filling in the fields ofone directly. On exit, the voice specification structure pointedto by the `voice` parameter containsthe appropriate values. You should never set the fields of sucha structure directly.

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

func GetVoiceInfo(UnsafePointer&lt;VoiceSpec>?, OSType, UnsafeMutableRawPointer) -> OSErr

Gets the same information about a voice that the `GetVoiceDescription` function provides,or to determine in which file and resource a voice is stored.

Deprecated

