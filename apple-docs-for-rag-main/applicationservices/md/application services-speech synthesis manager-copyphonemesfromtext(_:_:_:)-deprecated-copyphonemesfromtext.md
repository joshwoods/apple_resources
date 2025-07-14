

- Application Services
- Speech Synthesis Manager
-  CopyPhonemesFromText(\_:\_:\_:) Deprecated

Function

# CopyPhonemesFromText(\_:\_:\_:)

Converts the specified text string into its equivalent phonemic representation.

macOS 10.5–13.0Deprecated

``` source
func CopyPhonemesFromText(
    _ chan: SpeechChannel,
    _ text: CFString,
    _ phonemes: UnsafeMutablePointer
) -> OSErr
```

## Parameters 

`chan`  

A speech channel whose associated synthesizer and properties are to be used in the conversion process.

`text`  

The text from which to extract phonemic data.

`phonemes`  

On return, a `CFString` object that contains the extracted phonemic data. The caller is responsible for releasing this object.

## Return Value

A result code. See Result Codes.

## Discussion

The `CopyPhonemesFromText` function is the Core Foundation-based equivalent of the TextToPhonemes function.

Converting textual data into phonemic data is particularly useful during application development, when you might wish to adjust phrases that your application generates to produce smoother speech. By first converting the target phrase into phonemes, you can see what the synthesizer will try to speak. Then you need correct only the parts that would not have been spoken the way you want.

The data the `CopyPhonemesFromText` function stores in the `phonemes` parameter corresponds precisely to the phonemes that would be spoken had the input text been sent to `SpeakCFString` instead. All current property settings for the speech channel specified by `chan` are applied to the converted speech. No callbacks are generated while the `CopyPhonemesFromText` function is generating its output.

