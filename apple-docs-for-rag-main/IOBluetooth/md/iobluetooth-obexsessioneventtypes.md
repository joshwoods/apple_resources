

- IOBluetooth
-  OBEXSessionEventTypes 

Structure

# OBEXSessionEventTypes

Type identifiers for OBEX sessions.

macOS

``` source
struct OBEXSessionEventTypes
```

## Overview

When a new session event occurs, your selector (or C callback) will be given an OBEXSessionEvent pointer, and in it will be a ‘type’ field with one of the following types in it. Based on that type, you can then read the corresponding field in the union to get out interesting data for that event type. For example, if the type of an event is a ‘kOBEXSessionEventTypeConnectCommandResponseReceived’, you should look in the ‘OBEXConnectCommandResponseData’ part of the structure’s union to find more information pased to you in the event. Note that some you will never see, depending on the type of session you are using - a client or server. If you are a client (most likely case), you will never see the “Command” events, but instead you will only receive the “CommandResponse” events since you will be the issuer oft he commands, not the receiver of them. Both types of sessions will receive error type events.

## Topics

### Constants

var kOBEXSessionEventTypeAbortCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeAbortCommandResponseReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeConnectCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeConnectCommandResponseReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeDisconnectCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeDisconnectCommandResponseReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeError: OBEXSessionEventTypes

var kOBEXSessionEventTypeGetCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeGetCommandResponseReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypePutCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypePutCommandResponseReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeSetPathCommandReceived: OBEXSessionEventTypes

var kOBEXSessionEventTypeSetPathCommandResponseReceived: OBEXSessionEventTypes

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

