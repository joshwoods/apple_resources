

- Application Services
- Speech Synthesis Manager
-  CountVoices(\_:) Deprecated

Function

# CountVoices(\_:)

Determines how many voices are available.

macOS 10.0–13.0Deprecated

``` source
func CountVoices(_ numVoices: UnsafeMutablePointer) -> OSErr
```

## Parameters 

`numVoices`  

On exit, a pointer to the number of voices that the application can use.

## Return Value

A resultcode. See Result Codes.

## Discussion

The `CountVoices` functionreturns, in the `numVoices` parameter,the number of voices available. The application can then use thisinformation to call the `GetIndVoice` functionto obtain voice specification structures for one or more of thevoices.

Each time `CountVoices` iscalled, the Speech Synthesis Manager searches for new voices.

## See Also

### Getting Information About Voices

func GetIndVoice(Int16, UnsafeMutablePointer&lt;VoiceSpec>) -> OSErr

Gets a voice specification structure for a voice bypassing an index to the `GetIndVoice` function.

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

