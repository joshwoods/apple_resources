

- Audio Toolbox
- AUAudioUnitBus
-  init(format:) 

Initializer

# init(format:)

Initializes a bus object with a specific format.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(format: AVAudioFormat) throws
```

## Parameters 

`format`  

The initial audio format.

## Return Value

A newly-initialized bus object, or `nil` if the operation failed.

## Discussion

Audio units can generally be expected to support the AVAudioFormat standard format (deinterleaved 32-bit float), at any sample rate.

Channel counts can be more complex. See the channelCapabilities reference for a more complete discussion.

Initialization will fail and return an error if the specified format is unsupported for the bus.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Audio Unit Implementations

var supportedChannelCounts: [NSNumber]?

An array of numbers indicating the supported number of channels for this bus.

var maximumChannelCount: AUAudioChannelCount

The maximum number of channels supported for this bus.

