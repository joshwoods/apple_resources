

- IOBluetooth
-  OBEXNonceFlagValues 

Structure

# OBEXNonceFlagValues

Flags for Nonce command during digest challenge.

macOS

``` source
struct OBEXNonceFlagValues
```

## Topics

### Constants

var kOBEXNonceFlag2Reserved: OBEXNonceFlagValues

var kOBEXNonceFlag3Reserved: OBEXNonceFlagValues

var kOBEXNonceFlag4Reserved: OBEXNonceFlagValues

var kOBEXNonceFlag5Reserved: OBEXNonceFlagValues

var kOBEXNonceFlag6Reserved: OBEXNonceFlagValues

var kOBEXNonceFlag7Reserved: OBEXNonceFlagValues

var kOBEXNonceFlagAccessModeReadOnly: OBEXNonceFlagValues

var kOBEXNonceFlagNone: OBEXNonceFlagValues

var kOBEXNonceFlagSendUserIDInResponse: OBEXNonceFlagValues

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

