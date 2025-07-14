

- Application Services
- ApplicationServices Functions
-  TextToPhonemes(\_:\_:\_:\_:\_:) Deprecated

Function

# TextToPhonemes(\_:\_:\_:\_:\_:)

Mac Catalyst 16.0–16.0DeprecatedXcode 14.0–14.0Deprecated

``` source
func TextToPhonemes(
    _ chan: SpeechChannel,
    _ textBuf: UnsafeRawPointer,
    _ textBytes: UInt,
    _ phonemeBuf: Handle,
    _ phonemeBytes: UnsafeMutablePointer
) -> OSErr
```

