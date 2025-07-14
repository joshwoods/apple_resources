

- System
- Errno
-  rpcProcedureUnavailable 

Type Property

# rpcProcedureUnavailable

Bad procedure for program.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var rpcProcedureUnavailable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A remote procedure call was attempted for a procedure that doesn’t exist in the remote program.

The corresponding C error is `EPROCUNAVAIL`.

## See Also

### RPC Errors

static var rpcProgramUnavailable: Errno

The remote procedure call (RPC) program isn’t available.

static var rpcProgramVersionMismatch: Errno

The version of the remote procedure call (RPC) program is incorrect.

static var rpcUnsuccessful: Errno

The structure of the remote procedure call (RPC) is bad.

static var rpcVersionMismatch: Errno

The version of the remote procedure call (RPC) is incorrect.

