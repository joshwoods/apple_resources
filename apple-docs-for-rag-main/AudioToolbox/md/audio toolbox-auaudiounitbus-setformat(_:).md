

- Audio Toolbox
- AUAudioUnitBus
-  setFormat(\_:) 

Instance Method

# setFormat(\_:)

Sets the bus’s audio format.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setFormat(_ format: AVAudioFormat) throws
```

## Parameters 

`format`  

The desired audio format.

## Discussion

- false if the operation failed.

## Discussion

Audio units can generally be expected to support the AVAudioFormat standard format (deinterleaved 32-bit float), at any sample rate.

Channel counts can be more complex. See the channelCapabilities reference for a more complete discussion.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Bus Methods and Properties

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

var shouldAllocateBuffer: Bool

