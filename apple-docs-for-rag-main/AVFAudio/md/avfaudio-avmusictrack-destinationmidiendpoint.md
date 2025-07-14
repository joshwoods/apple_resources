

- AVFAudio
- AVMusicTrack
-  destinationMIDIEndpoint 

Instance Property

# destinationMIDIEndpoint

The MIDI endpoint you specify as the track’s target.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var destinationMIDIEndpoint: MIDIEndpointRef { get set }
```

## Discussion

This property and a destinationAudioUnit are mutually exclusive. Setting this property removes the track’s reference to an AVAudioUnit destination. When playing, the track sends events to the MIDI endpoint. For more information, see MIDIDestinationCreate(_:_:_:_:_:). You can’t change the endpoint while the track’s sequence is in a playing state.

## See Also

### Configuring the Track Destinations

var destinationAudioUnit: AVAudioUnit?

The audio unit that receives the track’s events.

