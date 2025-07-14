

- Audio Toolbox
-  AUHostMusicalContextBlock 

Type Alias

# AUHostMusicalContextBlock

A block through which hosts provide musical tempo, time signature, and beat position.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUHostMusicalContextBlock = (UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?) -> Bool
```

## Discussion

If the host app provides this block to an audio unit, via the musicalContextBlock property, then the block may be called at the beginning of each render cycle to obtain information about the current render cycle’s musical context. Any of the provided parameters may be null to indicate that the audio unit is not interested in that particular piece of information.

This block returns true if the operation was successful and false otherwise.

The block takes the following parameters:

currentTempo  
The current tempo, in beats per minute.

timeSignatureNumerator  
The numerator of the current time signature.

timeSignatureDenominator  
The denominator of the current time signature.

currentBeatPosition  
The precise beat position of the beginning of the current buffer being rendered.

sampleOffsetToNextBeat  
The number of samples between the beginning of the buffer being rendered and the next beat. Can be `0`.

currentMeasureDownbeatPosition  
The beat position corresponding to the beginning of the current measure.

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

typealias AUHostTransportStateBlock

A block through which hosts provide information about their transport state.

