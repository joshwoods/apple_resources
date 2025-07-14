

- AccessorySetupKit
- ASAccessory
-  ASAccessory.SupportOptions 

Structure

# ASAccessory.SupportOptions

Options of discoverable accessories.

iOS 18.0+iPadOS 18.0+

``` source
struct SupportOptions
```

## Topics

### Creating an options instance

init(rawValue: UInt)

### Bluetooth options

static var bluetoothPairingLE: ASAccessory.SupportOptions

The accessory supports Bluetooth Low Energy pairing.

static var bluetoothTransportBridging: ASAccessory.SupportOptions

The accessory supports bridging to Bluetooth classic transport.

static var bluetoothHID: ASAccessory.SupportOptions

The accessory supports Bluetooth Low Energy HID service.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Specifying options

var supportedOptions: ASAccessory.SupportOptions

Options supported by an accessory.

