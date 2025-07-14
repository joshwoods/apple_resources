

- System
-  Errno 

Structure

# Errno

An error number used by system calls to communicate what kind of error occurred.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct Errno
```

## Topics

### File and Directory Errors

static var attributeNotFound: Errno

Attribute not found.

static var badFileDescriptor: Errno

Bad file descriptor.

static var fileExists: Errno

File exists.

static var fileTooLarge: Errno

The file is too large.

static var improperLink: Errno

Improper link.

static var isDirectory: Errno

Is a directory.

static var noLocks: Errno

No locks available.

static var noSuchFileOrDirectory: Errno

No such file or directory.

static var notDirectory: Errno

Not a directory.

static var permissionDenied: Errno

Permission denied.

static var textFileBusy: Errno

Text file busy.

### File System Errors

static var badFileTypeOrFormat: Errno

Inappropriate file type or format.

static var directoryNotEmpty: Errno

Directory not empty.

static var diskQuotaExceeded: Errno

Disk quota exceeded.

static var noSpace: Errno

Device out of space.

static var readOnlyFileSystem: Errno

Read-only file system.

static var tooManyLinks: Errno

Too many links.

static var tooManyOpenFilesInSystem: Errno

The system has too many open files.

static var tooManyOpenFiles: Errno

This process has too many open files.

### NFS Errors

static var authenticationError: Errno

Authentication error.

static var needAuthenticator: Errno

Need authenticator.

static var staleNFSFileHandle: Errno

Stale NFS file handle.

### Device Errors

static var deviceError: Errno

Device error.

static var devicePowerIsOff: Errno

Device power is off.

static var inappropriateIOCTLForDevice: Errno

Inappropriate control function.

static var ioError: Errno

Input/output error.

static var noSuchAddressOrDevice: Errno

No such device or address.

static var notBlockDevice: Errno

Not a block device.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

### Path Errors

static var fileNameTooLong: Errno

The file name is too long.

static var tooManyRemoteLevels: Errno

Too many levels of remote in path.

static var tooManySymbolicLinkLevels: Errno

Too many levels of symbolic links.

### Pipe Errors

static var brokenPipe: Errno

Broken pipe.

static var illegalSeek: Errno

Illegal seek.

### Runtime Errors

static var deadlock: Errno

Resource deadlock avoided.

static var noMemory: Errno

Can’t allocate memory.

static var wouldBlock: Errno

Operation would block.

### Math Errors

static var outOfDomain: Errno

Numerical argument out of domain.

static var outOfRange: Errno

Numerical result out of range.

static var overflow: Errno

Value too large to be stored in data type.

### Executable File Errors

static var badCPUType: Errno

Bad CPU type in executable.

static var badExecutable: Errno

Bad executable or shared library.

static var execFormatError: Errno

Executable format error.

static var malformedMachO: Errno

Malformed Mach-O file.

static var sharedLibraryVersionMismatch: Errno

Shared library version mismatch.

### Network Errors

static var connectionAbort: Errno

Software caused a connection abort.

static var connectionRefused: Errno

Connection refused.

static var connectionReset: Errno

Connection reset by peer.

static var hostIsDown: Errno

The host is down.

static var messageTooLong: Errno

Message too long.

static var networkDown: Errno

Network is down.

static var networkReset: Errno

Network dropped connection on reset.

static var networkUnreachable: Errno

Network is unreachable.

static var noBufferSpace: Errno

No buffer space available.

static var noRouteToHost: Errno

No route to host.

static var notSupported: Errno

Not supported.

static var timedOut: Errno

Operation timed out.

### Network Protocol Errors

static var protocolError: Errno

Protocol error.

static var protocolFamilyNotSupported: Errno

Protocol family not supported.

static var protocolNotAvailable: Errno

Protocol not available.

static var protocolNotSupported: Errno

Protocol not supported.

static var protocolWrongTypeForSocket: Errno

Protocol wrong for socket type.

### Network Address Errors

static var addressFamilyNotSupported: Errno

The address family isn’t supported by the protocol family.

static var addressInUse: Errno

Address already in use.

static var addressNotAvailable: Errno

Can’t assign the requested address.

static var addressRequired: Errno

Destination address required.

### Network Socket Errors

static var notSocket: Errno

A socket operation was performed on something that isn’t a socket.

static var notSupportedOnSocket: Errno

Operation not supported on socket.

static var socketIsConnected: Errno

Socket is already connected.

static var socketNotConnected: Errno

Socket is not connected.

static var socketShutdown: Errno

Can’t send after socket shutdown.

static var socketTypeNotSupported: Errno

Socket type not supported.

### RPC Errors

static var rpcProcedureUnavailable: Errno

Bad procedure for program.

static var rpcProgramUnavailable: Errno

The remote procedure call (RPC) program isn’t available.

static var rpcProgramVersionMismatch: Errno

The version of the remote procedure call (RPC) program is incorrect.

static var rpcUnsuccessful: Errno

The structure of the remote procedure call (RPC) is bad.

static var rpcVersionMismatch: Errno

The version of the remote procedure call (RPC) is incorrect.

### Process Errors

static var argListTooLong: Errno

The argument list is too long.

static var identifierRemoved: Errno

Identifier removed.

static var noChildProcess: Errno

No child processes.

static var noSuchProcess: Errno

No such process.

static var previousOwnerDied: Errno

Previous pthread mutex owner died.

static var tooManyProcesses: Errno

Too many processes.

### System Call Errors

static var alreadyInProcess: Errno

Operation already in progress.

static var badAddress: Errno

Bad address.

static var interrupted: Errno

Interrupted function call.

static var invalidArgument: Errno

Invalid argument.

static var noFunction: Errno

Function not implemented.

static var nowInProgress: Errno

Operation now in progress.

static var resourceBusy: Errno

Resource busy.

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

### General Errors

static var badMessage: Errno

Bad message.

static var canceled: Errno

Operation canceled.

static var illegalByteSequence: Errno

Illegal byte sequence.

static var noData: Errno

No message available.

static var noMessage: Errno

No message of desired type.

static var noSuchPolicy: Errno

No such policy registered.

static var notPermitted: Errno

Operation not permitted.

static var notRecoverable: Errno

State not recoverable.

static var outputQueueFull: Errno

Interface output queue is full.

static var tooManyReferences: Errno

Too many references: can’t splice.

static var tooManyUsers: Errno

Too many users.

### Reserved

static var lastErrnoValue: Errno

The largest valid error.

static var multiHop: Errno

Reserved.

static var noLink: Errno

Reserved.

static var noStreamResources: Errno

Reserved.

static var notStream: Errno

Reserved.

static var notUsed: Errno

Error. Not used.

static var timeout: Errno

Reserved.

### Interacting with C APIs

init(rawValue: CInt)

Creates a strongly typed error number from a raw C error number.

let rawValue: CInt

The raw C error number.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Debugging

var description: String

A textual representation of the most recent error returned by a system call.

var debugDescription: String

A textual representation, suitable for debugging, of the most recent error returned by a system call.

### Encoding Errors

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int32`.

### Comparing Errors

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ~= (Errno, any Error) -> Bool

func hash(into: inout Hasher)

var hashValue: Int

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Error
- Hashable
- RawRepresentable
- Sendable

