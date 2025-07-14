

- IOBluetooth
-  OBEXError 

Type Alias

# OBEXError

Codes for OBEX errors. If the return value was not in the following range, then it is most likely resulting from kernel code/IOKit, and you should consult IOReturn.h for those codes.

macOS

``` source
typealias OBEXError = Int32
```

## Topics

### Constants

var kOBEXErrorRangeMin: OBEXErrorCodes

var kOBEXErrorRangeMax: OBEXErrorCodes

## See Also

### Related Documentation

typealias OBEXError

Codes for OBEX errors. If the return value was not in the following range, then it is most likely resulting from kernel code/IOKit, and you should consult IOReturn.h for those codes.

### Constants

struct OBEXConnectFlagValues

Flags for Connect command.

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

