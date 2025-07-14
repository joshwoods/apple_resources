

- Audio Toolbox
- AudioComponentDescription
-  componentType 

Instance Property

# componentType

A unique 4-byte code identifying the interface for the component.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var componentType: OSType
```

## See Also

### Properties

var componentSubType: OSType

A 4-byte code that you can use to indicate the purpose of a component. For example, you could use `lpas` or `lowp` as a mnemonic indication that an audio unit is a low-pass filter.

var componentManufacturer: OSType

The unique vendor identifier, registered with Apple, for the audio component.

var componentFlags: UInt32

Set this value to zero.

var componentFlagsMask: UInt32

Set this value to zero.

