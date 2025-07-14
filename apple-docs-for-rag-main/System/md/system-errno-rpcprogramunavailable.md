

- System
- Errno
-  rpcProgramUnavailable 

Type Property

# rpcProgramUnavailable

The remote procedure call (RPC) program isn’t available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var rpcProgramUnavailable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The requested program isn’t registered on the remote host.

The corresponding C error is `EPROGUNAVAIL`.

## See Also

### RPC Errors

static var rpcProcedureUnavailable: Errno

Bad procedure for program.

static var rpcProgramVersionMismatch: Errno

The version of the remote procedure call (RPC) program is incorrect.

static var rpcUnsuccessful: Errno

The structure of the remote procedure call (RPC) is bad.

static var rpcVersionMismatch: Errno

The version of the remote procedure call (RPC) is incorrect.

