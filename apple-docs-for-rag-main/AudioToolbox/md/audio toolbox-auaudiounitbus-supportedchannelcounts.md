

- Audio Toolbox
- AUAudioUnitBus
-  supportedChannelCounts 

Instance Property

# supportedChannelCounts

An array of numbers indicating the supported number of channels for this bus.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var supportedChannelCounts: [NSNumber]? { get set }
```

## Discussion

If the value of this property is `nil`, then any number less than or equal to the value of maximumChannelCount is supported. If setting a new value on this property makes the current bus format unsupported, then the value of format is set to `nil`.

The default value is `nil`.

## See Also

### Audio Unit Implementations

init(format: AVAudioFormat) throws

Initializes a bus object with a specific format.

var maximumChannelCount: AUAudioChannelCount

The maximum number of channels supported for this bus.

