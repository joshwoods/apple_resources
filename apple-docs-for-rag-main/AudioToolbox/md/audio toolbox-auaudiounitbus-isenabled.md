

- Audio Toolbox
- AUAudioUnitBus
-  isEnabled 

Instance Property

# isEnabled

Determines whether the bus is active.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

Hosts must enable input busses before using them. This allows an audio unit to be prepared to render a large number of inputs, but avoid the work of preparing to pull inputs which are not in use.

This version 3 property is bridged to the version 2 `kAudioUnitProperty_MakeConnection` and `kAudioUnitProperty_SetRenderCallback` APIs.

## See Also

### Bus Methods and Properties

func setFormat(AVAudioFormat) throws

Sets the bus’s audio format.

var format: AVAudioFormat

The audio format and channel layout of audio being transferred on the bus.

var name: String?

A name for the bus.

var index: Int

The index of this bus in its containing array.

var busType: AUAudioUnitBusType

The bus type.

var ownerAudioUnit: AUAudioUnit

The audio unit that owns the bus.

var supportedChannelLayoutTags: [NSNumber]?

An array of audio channel layout tags.

var contextPresentationLatency: TimeInterval

Information about latency in the audio unit’s processing context.

var shouldAllocateBuffer: Bool

