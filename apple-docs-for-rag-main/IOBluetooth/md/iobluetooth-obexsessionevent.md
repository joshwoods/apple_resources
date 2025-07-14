

- IOBluetooth
-  OBEXSessionEvent 

Structure

# OBEXSessionEvent

macOS

``` source
struct OBEXSessionEvent
```

## Overview

When a new session event occurs, your selector (or C callback) will be given an OBEXSessionEvent pointer, and in it will be information you might find interesting so that you can then reply back appropriately. For example, of you receive a kOBEXSessionEventTypeConnectCommandResponseReceived event, you can then parse out the information related to that event, and if all looks well to you, you could them send a “Get” command to get a file off of the OBEX server you just connected to.

## Topics

### Initializers

init()

init(type: OBEXSessionEventType, session: OBEXSessionRef!, refCon: UnsafeMutableRawPointer!, isEndOfEventData: DarwinBoolean, reserved1: UnsafeMutableRawPointer!, reserved2: UnsafeMutableRawPointer!, u: OBEXSessionEvent.__Unnamed_union_u)

### Instance Properties

var isEndOfEventData: DarwinBoolean

var refCon: UnsafeMutableRawPointer!

var reserved1: UnsafeMutableRawPointer!

var reserved2: UnsafeMutableRawPointer!

var session: OBEXSessionRef!

var type: OBEXSessionEventType

var u: OBEXSessionEvent.__Unnamed_union_u

## See Also

### Data Types

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

