

- Application Services
- ApplicationServices Functions
-  InvokeSpeechTextDoneUPP(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# InvokeSpeechTextDoneUPP(\_:\_:\_:\_:\_:\_:)

Mac Catalyst 16.0–16.0DeprecatedXcode 14.0–14.0Deprecated

``` source
func InvokeSpeechTextDoneUPP(
    _ chan: SpeechChannel,
    _ refCon: SRefCon,
    _ nextBuf: UnsafeMutablePointer?,
    _ byteLen: UnsafeMutablePointer,
    _ controlFlags: UnsafeMutablePointer,
    _ userUPP: SpeechTextDoneUPP
)
```

