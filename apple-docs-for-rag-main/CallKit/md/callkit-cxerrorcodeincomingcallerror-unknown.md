

- CallKit
- CXErrorCodeIncomingCallError
-  unknown 

Type Property

# unknown

An unknown error occurred.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
static var unknown: CXErrorCodeIncomingCallError.Code { get }
```

## See Also

### Errors

static var callUUIDAlreadyExists: CXErrorCodeIncomingCallError.Code

The incoming call UUID already exists.

static var filteredByBlockList: CXErrorCodeIncomingCallError.Code

The system is filtering the incoming call because the user is blocking it.

static var filteredByDoNotDisturb: CXErrorCodeIncomingCallError.Code

The system is filtering the incoming call because Do Not Disturb is active and the incoming caller isn’t a VIP.

static var unentitled: CXErrorCodeIncomingCallError.Code

The app doesn’t have the entitlement to receive incoming calls.

