

- Audio Toolbox
- AUAudioUnitBus
-  name 

Instance Property

# name

A name for the bus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var name: String? { get set }
```

## Discussion

The bus name can be set by the host.

## See Also

### Bus Methods and Properties

func setFormat(AVAudioFormat) throws

Sets the bus’s audio format.

var format: AVAudioFormat

The audio format and channel layout of audio being transferred on the bus.

var isEnabled: Bool

Determines whether the bus is active.

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

