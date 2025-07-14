

- Application Services
- Speech Synthesis Manager
- VoiceSpec
-  creator 

Instance Property

# creator

The synthesizer that is required to use the voice. This is equivalent to the value contained in the `synthManufacturer` field of a speech version information structure and that contained in the `synthCreator` field of a speech extension data structure. The set of `OSType` values specified entirely by space characters and lowercase letters is reserved.

macOS 10.0+

``` source
var creator: OSType
```

