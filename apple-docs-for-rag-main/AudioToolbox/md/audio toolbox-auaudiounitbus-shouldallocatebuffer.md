

- Audio Toolbox
- AUAudioUnitBus
-  shouldAllocateBuffer 

Instance Property

# shouldAllocateBuffer

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var shouldAllocateBuffer: Bool { get set }
```

## See Also

### Bus Methods and Properties

func setFormat(AVAudioFormat) throws

Sets the bus’s audio format.

var format: AVAudioFormat

The audio format and channel layout of audio being transferred on the bus.

var isEnabled: Bool

Determines whether the bus is active.

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

