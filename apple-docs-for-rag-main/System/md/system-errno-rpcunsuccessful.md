

- System
- Errno
-  rpcUnsuccessful 

Type Property

# rpcUnsuccessful

The structure of the remote procedure call (RPC) is bad.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var rpcUnsuccessful: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Exchange of RPC information was unsuccessful.

The corresponding C error is `EBADRPC`.

## See Also

### RPC Errors

static var rpcProcedureUnavailable: Errno

Bad procedure for program.

static var rpcProgramUnavailable: Errno

The remote procedure call (RPC) program isn’t available.

static var rpcProgramVersionMismatch: Errno

The version of the remote procedure call (RPC) program is incorrect.

static var rpcVersionMismatch: Errno

The version of the remote procedure call (RPC) is incorrect.

