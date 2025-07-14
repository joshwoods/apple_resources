

- IOBluetooth
-  OBEXOpCodeCommandValues 

Structure

# OBEXOpCodeCommandValues

Operation OpCode values for commands.

macOS

``` source
struct OBEXOpCodeCommandValues
```

## Topics

### Constants

var kOBEXOpCodeAbort: OBEXOpCodeCommandValues

var kOBEXOpCodeConnect: OBEXOpCodeCommandValues

var kOBEXOpCodeDisconnect: OBEXOpCodeCommandValues

var kOBEXOpCodeGet: OBEXOpCodeCommandValues

var kOBEXOpCodeGetWithHighBitSet: OBEXOpCodeCommandValues

var kOBEXOpCodePut: OBEXOpCodeCommandValues

var kOBEXOpCodePutWithHighBitSet: OBEXOpCodeCommandValues

var kOBEXOpCodeReserved: OBEXOpCodeCommandValues

var kOBEXOpCodeReservedRangeEnd: OBEXOpCodeCommandValues

var kOBEXOpCodeReservedRangeStart: OBEXOpCodeCommandValues

var kOBEXOpCodeReservedWithHighBitSet: OBEXOpCodeCommandValues

var kOBEXOpCodeSetPath: OBEXOpCodeCommandValues

var kOBEXOpCodeUserDefinedEnd: OBEXOpCodeCommandValues

var kOBEXOpCodeUserDefinedStart: OBEXOpCodeCommandValues

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

typealias BluetoothAFHMode

typealias BluetoothAirMode

typealias BluetoothAllowRoleSwitch

typealias BluetoothAuthenticationRequirements

struct BluetoothAuthenticationRequirementsValues

typealias BluetoothClassOfDevice

typealias BluetoothClockOffset

struct BluetoothCompanyIdentifers

typealias BluetoothConnectionHandle

typealias BluetoothDeviceClassMajor

typealias BluetoothDeviceClassMinor

typealias BluetoothDeviceName

typealias BluetoothEncryptionEnable

struct BluetoothFeatureBits

typealias BluetoothHCIACLDataByteCount

