

- IOBluetooth
-  OBEXErrorData 

Structure

# OBEXErrorData

Part of the OBEXSessionEvent structure.

macOS

``` source
struct OBEXErrorData
```

## Overview

Is readable when the event is of type kOBEXSessionEventTypeError (see OBEXSessionEventTypes).

## Topics

### Initializers

init()

init(error: OBEXError, dataPtr: UnsafeMutableRawPointer!, dataLength: Int)

### Instance Properties

var dataLength: Int

var dataPtr: UnsafeMutableRawPointer!

var error: OBEXError

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

struct OBEXConnectCommandData

Part of the OBEXSessionEvent structure.

struct OBEXConnectCommandResponseData

Part of the OBEXSessionEvent structure.

struct OBEXDisconnectCommandData

Part of the OBEXSessionEvent structure.

struct OBEXDisconnectCommandResponseData

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

