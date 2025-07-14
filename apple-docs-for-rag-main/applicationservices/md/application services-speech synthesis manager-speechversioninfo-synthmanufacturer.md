

- Application Services
- Speech Synthesis Manager
- SpeechVersionInfo
-  synthManufacturer 

Instance Property

# synthManufacturer

A unique identification of a synthesizer engine. If you develop synthesizers, then you should register a different four-character code for each synthesizer you develop with Developer Technical Support. The `creatorID` field of the voice specification structure and the `synthCreator` field of a speech extension data structure should each be set to the value stored in this field for the desired synthesizer.

macOS 10.0+

``` source
var synthManufacturer: OSType
```

