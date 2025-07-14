

- IOBluetooth
-  OBEX.h 

API Collection

# OBEX.h

Public OBEX technology interfaces.

## Overview

Contains generic OBEX constants, structs, and C API used for all OBEX communication over any transport. For specific transport API, see that transport’s C API. For example, if you wanted to know more about the Bluetooth OBEX implementation, see OBEXBluetooth.h.

The file also contains API that will assist in the construction and deconstruction of OBEX headers to and from raw bytes, as well as the creation of vCards and vEvents.

### Included Headers

- \

- \

- \

- \

## Topics

### Miscellaneous

func OBEXAddApplicationParameterHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes representing an application parameter to a dictionary of OBEX headers.

func OBEXAddAuthorizationChallengeHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an authorization challenge header to a dictionary of OBEXheaders.

func OBEXAddAuthorizationResponseHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an authorization Response header to a dictionary of OBEXheaders.

func OBEXAddBodyHeader(UnsafeRawPointer!, UInt32, Bool, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddByteSequenceHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add a byte sequence header to a dictionary of OBEXheaders.

func OBEXAddConnectionIDHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes representing a connection ID to a dictionary of OBEX headers.

func OBEXAddCountHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddDescriptionHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddHTTPHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddLengthHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddNameHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddObjectClassHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an object class header to a dictionary of OBEXheaders.

func OBEXAddTargetHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddTime4ByteHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddTimeISOHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes to a dictionary of OBEXheaders.

func OBEXAddTypeHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddUserDefinedHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add a user-defined custom header to a dictionary of OBEXheaders.

func OBEXAddWhoHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXGetHeaders(UnsafeRawPointer!, Int) -> CFDictionary!

Take a data blob and looks for OBEX headers.

func OBEXHeadersToBytes(CFDictionary!) -> Unmanaged&lt;CFMutableData>!

Converts a dictionary of headers to a data pointer, from which you can extract as bytes and pass to the OBEX command/response functions.

### Data Types

See the Overview for header-level documentation.

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

### Constants

See the Overview for header-level documentation.

struct OBEXConnectFlagValues

Flags for Connect command.

typealias OBEXError

Codes for OBEX errors. If the return value was not in the following range, then it is most likely resulting from kernel code/IOKit, and you should consult IOReturn.h for those codes.

struct OBEXHeaderIdentifiers

Identifiers for OBEX Headers.

struct OBEXNonceFlagValues

Flags for Nonce command during digest challenge.

struct OBEXOpCodeCommandValues

Operation OpCode values for commands.

struct OBEXOpCodeResponseValues

Response opCode values.

struct OBEXOpCodeSessionValues

Operation OpCode values for sessions. From the OBEX 1.3 specification.

struct OBEXPutFlagValues

struct OBEXRealmValues

Values for Realm during digest response.

struct OBEXSessionEventTypes

Type identifiers for OBEX sessions.

struct OBEXSessionParameterTags

Tags for SessionParameters.

struct OBEXVersions

The available/supported OBEX versions.

### Macros

OBEX Convenience Macros

Convenience Macros for working with OBEX Header Identifiers.

## See Also

### Reference

Bluetooth.h User-Space

Bluetooth wireless technology

IOBluetoothUserLib.h

Public Interfaces for Apple’s implementation of Bluetooth technology.

IOBluetoothUtilities.h

See the Overview section above for header-level documentation.

OBEXBluetooth.h

Object Exchange over Bluetooth.

OBEXFileTransferServices.h

IOBluetooth Structures

IOBluetooth Enumerations

IOBluetooth Constants

IOBluetooth Functions

IOBluetooth Data Types

