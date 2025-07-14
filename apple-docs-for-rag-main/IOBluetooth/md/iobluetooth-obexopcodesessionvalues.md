

- IOBluetooth
-  OBEXOpCodeSessionValues 

Structure

# OBEXOpCodeSessionValues

Operation OpCode values for sessions. From the OBEX 1.3 specification.

macOS

``` source
struct OBEXOpCodeSessionValues
```

## Topics

### Constants

var kOBEXOpCodeCloseSession: OBEXOpCodeSessionValues

var kOBEXOpCodeCreateSession: OBEXOpCodeSessionValues

var kOBEXOpCodeResumeSession: OBEXOpCodeSessionValues

var kOBEXOpCodeSetTimeout: OBEXOpCodeSessionValues

var kOBEXOpCodeSuspendSession: OBEXOpCodeSessionValues

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

