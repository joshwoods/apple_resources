

- AVFAudio
- AVAudioSessionRouteDescription
-  inputs 

Instance Property

# inputs

An array of audio input port descriptions.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var inputs: [AVAudioSessionPortDescription] { get }
```

## Discussion

This property contains an array of AVAudioSessionPortDescription objects representing the audio inputs associated with the current audio route for a session.

## See Also

### Getting the Input and Output Ports

var outputs: [AVAudioSessionPortDescription]

An array of audio output port descriptions.

