

- Application Services
- Speech Synthesis Manager
-  SetSpeechProperty(\_:\_:\_:) Deprecated

Function

# SetSpeechProperty(\_:\_:\_:)

Sets the value of the specified speech-channel property.

macOS 10.5–13.0Deprecated

``` source
func SetSpeechProperty(
    _ chan: SpeechChannel,
    _ property: CFString,
    _ object: CFTypeRef?
) -> OSErr
```

## Parameters 

`chan`  

The speech channel whose property to set.

`property`  

The speech-channel property to set to the specified value.

`object`  

The value to which the specified speech-channel property should be set. For some properties, this value can be `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

The `SetSpeechProperty` function is the Core Foundation-based equivalent of the SetSpeechInfo function.

See Speech-Channel Properties for information on the properties you can specify.

## See Also

### Changing Speech Attributes

func SetSpeechPitch(SpeechChannel, Fixed) -> OSErr

Sets the speech pitch on a designated speech channel.

Deprecated

func SetSpeechRate(SpeechChannel, Fixed) -> OSErr

Sets the speech rate of a designated speech channel.

Deprecated

