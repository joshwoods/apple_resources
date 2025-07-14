

- Audio Toolbox
- AUAudioUnitBus
-  maximumChannelCount 

Instance Property

# maximumChannelCount

The maximum number of channels supported for this bus.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var maximumChannelCount: AUAudioChannelCount { get set }
```

## Discussion

If the value of supportedChannelCounts is set, then this value is derived from it. If setting a new value on this property makes the current bus format unsupported, then the value of format is set to `nil`.

The default value is `UINT_MAX`.

## See Also

### Audio Unit Implementations

init(format: AVAudioFormat) throws

Initializes a bus object with a specific format.

var supportedChannelCounts: [NSNumber]?

An array of numbers indicating the supported number of channels for this bus.

