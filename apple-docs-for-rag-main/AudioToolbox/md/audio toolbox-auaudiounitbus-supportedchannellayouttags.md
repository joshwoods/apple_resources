

- Audio Toolbox
- AUAudioUnitBus
-  supportedChannelLayoutTags 

Instance Property

# supportedChannelLayoutTags

An array of audio channel layout tags.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var supportedChannelLayoutTags: [NSNumber]? { get }
```

## Discussion

The array contains NSNumber objects representing AudioChannelLayoutTag values.

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

var contextPresentationLatency: TimeInterval

Information about latency in the audio unit’s processing context.

var shouldAllocateBuffer: Bool

