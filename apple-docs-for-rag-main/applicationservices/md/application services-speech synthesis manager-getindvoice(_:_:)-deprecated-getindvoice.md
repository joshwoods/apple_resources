

- Application Services
- Speech Synthesis Manager
-  GetIndVoice(\_:\_:) Deprecated

Function

# GetIndVoice(\_:\_:)

Gets a voice specification structure for a voice bypassing an index to the `GetIndVoice` function.

macOS 10.0–13.0Deprecated

``` source
func GetIndVoice(
    _ index: Int16,
    _ voice: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`index`  

The index of the voice for which to obtain a voice specification structure. This number must range from `1` to the total number of voices, as returned by the `CountVoices` function.

`voice`  

A pointer to the voice specification structure whose fields are to be filled in.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `GetIndVoice` functionreturns, in the voice specification structure pointed to by the `voice` parameter,a specification of the voice whose index is provided in the `index` parameter.Your application should make no assumptions about the order in whichvoices are indexed.

Your application should not add, remove, or modify a voiceand then call the `GetIndVoice` functionwith an index value other than `1`. To allow the Speech SynthesisManager to update its information about voices, your applicationshould always either call the `CountVoices` functionor call the `GetIndVoice` functionwith an index value of `1` after adding, removing, or modifying avoice or after a time at which the user might have done so.

If you specify an index value beyond the number of availablevoices, the `GetIndVoice` functionreturns a `voiceNotFound` error.

## See Also

### Getting Information About Voices

func CountVoices(UnsafeMutablePointer&lt;Int16>) -> OSErr

Determines how many voices are available.

Deprecated

func GetVoiceDescription(UnsafePointer&lt;VoiceSpec>?, UnsafeMutablePointer&lt;VoiceDescription>?, Int) -> OSErr

Gets a description of a voice by using the `GetVoiceDescription` function.

Deprecated

func GetVoiceInfo(UnsafePointer&lt;VoiceSpec>?, OSType, UnsafeMutableRawPointer) -> OSErr

Gets the same information about a voice that the `GetVoiceDescription` function provides,or to determine in which file and resource a voice is stored.

Deprecated

func MakeVoiceSpec(OSType, OSType, UnsafeMutablePointer&lt;VoiceSpec>) -> OSErr

Sets the fields of a voice specification structure.

Deprecated

