

- Bundle Resources
- Information Property List
-  NSAlwaysAllowMicrophoneModeControl 

Property List Key

# NSAlwaysAllowMicrophoneModeControl

A Boolean value that indicates if a person can configure a microphone mode regardless of whether the microphone is in an active state.

iOS 18.0+iPadOS 18.0+

## Details 

Type  

boolean

## Discussion

When your app is in the foreground, use this key to allow someone to configure their microphone mode — automatic, standard, voice isolation, or wide spectrum — before activating the microphone. For example, a person can configure the microphone mode to voice isolation before starting a call in your teleconferencing app.

