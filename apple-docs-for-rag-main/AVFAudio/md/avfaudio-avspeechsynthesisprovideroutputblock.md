

- AVFAudio
-  AVSpeechSynthesisProviderOutputBlock 

Type Alias

# AVSpeechSynthesisProviderOutputBlock

A type that represents the method for sending marker information to the host.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias AVSpeechSynthesisProviderOutputBlock = ([AVSpeechSynthesisMarker], AVSpeechSynthesisProviderRequest) -> Void
```

## Parameters 

`markers`  

An array of speech synthesis metadata.

`speechRequest`  

A speech request the system associates with the metadata.

## See Also

### Supplying metadata

var speechSynthesisOutputMetadataBlock: AVSpeechSynthesisProviderOutputBlock?

A block that subclasses use to send marker information to the host.

class AVSpeechSynthesisMarker

An object that contains information about the synthesized audio.

