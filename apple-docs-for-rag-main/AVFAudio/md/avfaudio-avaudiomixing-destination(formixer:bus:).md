

- AVFAudio
- AVAudioMixing
-  destination(forMixer:bus:) 

Instance Method

# destination(forMixer:bus:)

Gets the audio mixing destination object that corresponds to the specified mixer node and input bus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func destination(
    forMixer mixer: AVAudioNode,
    bus: AVAudioNodeBus
) -> AVAudioMixingDestination?
```

**Required**

## Parameters 

`mixer`  

The mixer to get destination details for.

`bus`  

The input bus.

## Return Value

Returns `self` if the specified mixer or input bus matches its connection point. If the mixer or input bus doesn’t match its connection point, or if the source node isn’t in a connected state to the mixer or input bus, the method returns `nil.`

## Discussion

When you connect a source node to multiple mixers downstream, setting AVAudioMixing properties directly on the source node applies the change to all of them. Use this method to get the corresponding AVAudioMixingDestination for a specific mixer. Properties set on individual destination instances don’t reflect at the source node level.

If there’s any disconnection between the source and mixer nodes, the return value can be invalid. Fetch the return value every time you want to set or get properties on a specific mixer.

## See Also

### Getting and Setting the Destination

class AVAudioMixingDestination

An object that represents a connection to a mixer node from a node that conforms to the audio mixing protocol.

