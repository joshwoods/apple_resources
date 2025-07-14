

- System
- Errno
-  rpcProgramVersionMismatch 

Type Property

# rpcProgramVersionMismatch

The version of the remote procedure call (RPC) program is incorrect.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var rpcProgramVersionMismatch: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The requested version of the program isn’t available on the remote host.

The corresponding C error is `EPROGMISMATCH`.

## See Also

### RPC Errors

static var rpcProcedureUnavailable: Errno

Bad procedure for program.

static var rpcProgramUnavailable: Errno

The remote procedure call (RPC) program isn’t available.

static var rpcUnsuccessful: Errno

The structure of the remote procedure call (RPC) is bad.

static var rpcVersionMismatch: Errno

The version of the remote procedure call (RPC) is incorrect.

