

- Audio Toolbox
- AUAudioUnit
-  musicalContextBlock 

Instance Property

# musicalContextBlock

A callback to the host for musical context information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var musicalContextBlock: AUHostMusicalContextBlock? { get set }
```

## Discussion

An audio unit accessing this property should cache it in realtime-safe storage before beginning to render.

This version 3 property is bridged to the version 2 HostCallback_GetBeatAndTempo and HostCallback_GetMusicalTimeLocation callback members in the `kAudioUnitProperty_HostCallbacks` API.

## See Also

### Providing Data to the Host

var transportStateBlock: AUHostTransportStateBlock?

A callback to the host for transport state information.

var contextName: String?

Information about the host context in which the audio unit is connected, for display in the audio unit’s view.

var supportsMPE: Bool

A Boolean value that indicates whether the audio unit supports multi-dimensional polyphonic expression.

typealias AUHostMusicalContextBlock

A block through which hosts provide musical tempo, time signature, and beat position.

typealias AUHostTransportStateBlock

A block through which hosts provide information about their transport state.

