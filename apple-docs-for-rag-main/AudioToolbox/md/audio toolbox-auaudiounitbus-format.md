

- Audio Toolbox
- AUAudioUnitBus
-  format 

Instance Property

# format

The audio format and channel layout of audio being transferred on the bus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var format: AVAudioFormat { get }
```

## Discussion

This version 3 property is bridged to the version 2 `kAudioUnitProperty_StreamFormat` API.

## See Also

### Bus Methods and Properties

func setFormat(AVAudioFormat) throws

Sets the bus’s audio format.

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

var shouldAllocateBuffer: Bool

