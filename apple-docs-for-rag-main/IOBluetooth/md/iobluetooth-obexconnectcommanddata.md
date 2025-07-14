

- IOBluetooth
-  OBEXConnectCommandData 

Structure

# OBEXConnectCommandData

Part of the OBEXSessionEvent structure.

macOS

``` source
struct OBEXConnectCommandData
```

## Overview

Is readable when the event is of type kOBEXSessionEventTypeConnectCommandReceived (see OBEXSessionEventTypes).

## Topics

### Initializers

init()

init(headerDataPtr: UnsafeMutableRawPointer!, headerDataLength: Int, maxPacketSize: OBEXMaxPacketLength, version: OBEXVersion, flags: OBEXFlags)

### Instance Properties

var flags: OBEXFlags

var headerDataLength: Int

var headerDataPtr: UnsafeMutableRawPointer!

var maxPacketSize: OBEXMaxPacketLength

var version: OBEXVersion

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct OBEXSessionEvent

struct OBEXAbortCommandData

Part of the OBEXSessionEvent structure.

struct OBEXAbortCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXConnectCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXDisconnectCommandData

Part of the OBEXSessionEvent structure.

struct OBEXDisconnectCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXErrorData

Part of the OBEXSessionEvent structure.

struct OBEXGetCommandData

Part of the OBEXSessionEvent structure.

struct OBEXGetCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXPutCommandData

Part of the OBEXSessionEvent structure.

struct OBEXPutCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXSetPathCommandData

Part of the OBEXSessionEvent structure.

struct OBEXSetPathCommandResponseData

Part of the OBEXSessionEvent structure.

