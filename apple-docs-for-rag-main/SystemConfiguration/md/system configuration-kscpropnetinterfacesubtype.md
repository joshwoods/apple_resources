

- System Configuration
-  kSCPropNetInterfaceSubType 

Global Variable

# kSCPropNetInterfaceSubType

The Interface key `SubType`, whose value is of type `CFString`.

macOS 10.1+

``` source
let kSCPropNetInterfaceSubType: CFString
```

## Discussion

This key can be passed the following constants when the `Type` key has the value `PPP`:

- `kSCValNetInterfaceSubTypePPPoE`, which has the value `PPPoE`

- `kSCValNetInterfaceSubTypePPPSerial`, which has the value `PPPSerial`

- `kSCValNetInterfaceSubTypePPTP`, which has the value `PPTP`

- `kSCValNetInterfaceSubTypeL2TP`, which has the value `L2TP`

## See Also

### Constants

let kSCPropNetInterfaceDeviceName: CFString

The Interface key `DeviceName`, whose value is of type `CFString`.

let kSCPropNetInterfaceHardware: CFString

The Interface key `Hardware`, whose value is of type `CFString`.

let kSCPropNetInterfaceType: CFString

The Interface key `Type`, whose value is of type `CFString`.

let kSCPropNetInterfaceSupportsModemOnHold: CFString

The Interface key `SupportsModemOnHold`, whose value is of type `CFNumber` and is equal to `0` or `1`.

Deprecated

