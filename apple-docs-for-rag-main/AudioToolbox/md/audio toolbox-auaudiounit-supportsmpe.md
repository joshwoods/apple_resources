

- Audio Toolbox
- AUAudioUnit
-  supportsMPE 

Instance Property

# supportsMPE

A Boolean value that indicates whether the audio unit supports multi-dimensional polyphonic expression.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var supportsMPE: Bool { get }
```

## See Also

### Providing Data to the Host

var musicalContextBlock: AUHostMusicalContextBlock?

A callback to the host for musical context information.

var transportStateBlock: AUHostTransportStateBlock?

A callback to the host for transport state information.

var contextName: String?

Information about the host context in which the audio unit is connected, for display in the audio unit’s view.

typealias AUHostMusicalContextBlock

A block through which hosts provide musical tempo, time signature, and beat position.

typealias AUHostTransportStateBlock

A block through which hosts provide information about their transport state.

