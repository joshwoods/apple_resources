

- Audio Toolbox
-  AUHostTransportStateBlock 

Type Alias

# AUHostTransportStateBlock

A block through which hosts provide information about their transport state.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUHostTransportStateBlock = (UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?) -> Bool
```

## Discussion

If the host app provides this block to an audio unit, via the transportStateBlock property, then the block may be called at the beginning of each render cycle to obtain information about the current transport state. Any of the provided parameters may be null to indicate that the audio unit is not interested in that particular piece of information.

This block returns true if the transport state was able to be retrieved from the host; it returns false otherwise.

The block takes the following parameters:

transportStateFlags  
The current state of the audio transport.

currentSamplePosition  
The current position in the host’s timeline, in samples at the audio unit’s output sample rate.

cycleStartBeatPosition  
If cycling, the starting beat position of the cycle.

cycleEndBeatPosition  
If cycling, the ending beat position of the cycle.

## See Also

### Providing Data to the Host

var musicalContextBlock: AUHostMusicalContextBlock?

A callback to the host for musical context information.

var transportStateBlock: AUHostTransportStateBlock?

A callback to the host for transport state information.

var contextName: String?

Information about the host context in which the audio unit is connected, for display in the audio unit’s view.

var supportsMPE: Bool

A Boolean value that indicates whether the audio unit supports multi-dimensional polyphonic expression.

typealias AUHostMusicalContextBlock

A block through which hosts provide musical tempo, time signature, and beat position.

