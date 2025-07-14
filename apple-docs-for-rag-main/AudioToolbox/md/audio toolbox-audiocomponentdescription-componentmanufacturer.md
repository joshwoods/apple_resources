

- Audio Toolbox
- AudioComponentDescription
-  componentManufacturer 

Instance Property

# componentManufacturer

The unique vendor identifier, registered with Apple, for the audio component.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var componentManufacturer: OSType
```

## See Also

### Properties

var componentType: OSType

A unique 4-byte code identifying the interface for the component.

var componentSubType: OSType

A 4-byte code that you can use to indicate the purpose of a component. For example, you could use `lpas` or `lowp` as a mnemonic indication that an audio unit is a low-pass filter.

var componentFlags: UInt32

Set this value to zero.

var componentFlagsMask: UInt32

Set this value to zero.

