

- Foundation
-  POSIXError 

Structure

# POSIXError

Describes an error in the POSIX error domain.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct POSIXError
```

## Topics

### Type Aliases

typealias Code

### Type Properties

static var E2BIG: POSIXErrorCode

Argument list too long.

static var EACCES: POSIXErrorCode

Permission denied.

static var EADDRINUSE: POSIXErrorCode

Address already in use.

static var EADDRNOTAVAIL: POSIXErrorCode

Can’t assign requested address.

static var EAFNOSUPPORT: POSIXErrorCode

Address family not supported by protocol family.

static var EAGAIN: POSIXErrorCode

non-blocking and interrupt i/o. Resource temporarily unavailable.

static var EALREADY: POSIXErrorCode

Operation already in progress.

static var EAUTH: POSIXErrorCode

Authentication error.

static var EBADARCH: POSIXErrorCode

Bad CPU type in executable.

static var EBADEXEC: POSIXErrorCode

Program loading errors. Bad executable.

static var EBADF: POSIXErrorCode

Bad file descriptor.

static var EBADMACHO: POSIXErrorCode

Malformed Macho file.

static var EBADMSG: POSIXErrorCode

Bad message.

static var EBADRPC: POSIXErrorCode

RPC struct is bad.

static var EBUSY: POSIXErrorCode

Device / Resource busy.

static var ECANCELED: POSIXErrorCode

Operation canceled.

static var ECHILD: POSIXErrorCode

No child processes.

static var ECONNABORTED: POSIXErrorCode

Software caused connection abort.

static var ECONNREFUSED: POSIXErrorCode

Connection refused.

static var ECONNRESET: POSIXErrorCode

Connection reset by peer.

static var EDEADLK: POSIXErrorCode

Resource deadlock avoided.

static var EDESTADDRREQ: POSIXErrorCode

Destination address required.

static var EDEVERR: POSIXErrorCode

Device error, for example paper out.

static var EDOM: POSIXErrorCode

math software. Numerical argument out of domain.

static var EDQUOT: POSIXErrorCode

Disc quota exceeded.

static var EEXIST: POSIXErrorCode

File exists.

static var EFAULT: POSIXErrorCode

Bad address.

static var EFBIG: POSIXErrorCode

File too large.

static var EFTYPE: POSIXErrorCode

Inappropriate file type or format.

static var EHOSTDOWN: POSIXErrorCode

Host is down.

static var EHOSTUNREACH: POSIXErrorCode

No route to host.

static var EIDRM: POSIXErrorCode

Identifier removed.

static var EILSEQ: POSIXErrorCode

Illegal byte sequence.

static var EINPROGRESS: POSIXErrorCode

Operation now in progress.

static var EINTR: POSIXErrorCode

Interrupted system call.

static var EINVAL: POSIXErrorCode

Invalid argument.

static var EIO: POSIXErrorCode

Input/output error.

static var EISCONN: POSIXErrorCode

Socket is already connected.

static var EISDIR: POSIXErrorCode

Is a directory.

static var ELOOP: POSIXErrorCode

Too many levels of symbolic links.

static var EMFILE: POSIXErrorCode

Too many open files.

static var EMLINK: POSIXErrorCode

Too many links.

static var EMSGSIZE: POSIXErrorCode

Message too long.

static var EMULTIHOP: POSIXErrorCode

Reserved.

static var ENAMETOOLONG: POSIXErrorCode

File name too long.

static var ENEEDAUTH: POSIXErrorCode

Need authenticator.

static var ENETDOWN: POSIXErrorCode

ipc/network software – operational errors Network is down.

static var ENETRESET: POSIXErrorCode

Network dropped connection on reset.

static var ENETUNREACH: POSIXErrorCode

Network is unreachable.

static var ENFILE: POSIXErrorCode

Too many open files in system.

static var ENOATTR: POSIXErrorCode

Attribute not found.

static var ENOBUFS: POSIXErrorCode

No buffer space available.

static var ENODATA: POSIXErrorCode

No message available on STREAM.

static var ENODEV: POSIXErrorCode

Operation not supported by device.

static var ENOENT: POSIXErrorCode

No such file or directory.

static var ENOEXEC: POSIXErrorCode

Exec format error.

static var ENOLCK: POSIXErrorCode

No locks available.

static var ENOLINK: POSIXErrorCode

Reserved.

static var ENOMEM: POSIXErrorCode

Cannot allocate memory.

static var ENOMSG: POSIXErrorCode

No message of desired type.

static var ENOPOLICY: POSIXErrorCode

No such policy registered.

static var ENOPROTOOPT: POSIXErrorCode

Protocol not available.

static var ENOSPC: POSIXErrorCode

No space left on device.

static var ENOSR: POSIXErrorCode

No STREAM resources.

static var ENOSTR: POSIXErrorCode

Not a STREAM.

static var ENOSYS: POSIXErrorCode

Function not implemented.

static var ENOTBLK: POSIXErrorCode

Block device required.

static var ENOTCONN: POSIXErrorCode

Socket is not connected.

static var ENOTDIR: POSIXErrorCode

Not a directory.

static var ENOTEMPTY: POSIXErrorCode

Directory not empty.

static var ENOTRECOVERABLE: POSIXErrorCode

State not recoverable.

static var ENOTSOCK: POSIXErrorCode

ipc/network software – argument errors. Socket operation on non-socket.

static var ENOTSUP: POSIXErrorCode

Operation not supported.

static var ENOTTY: POSIXErrorCode

Inappropriate ioctl for device.

static var ENXIO: POSIXErrorCode

Device not configured.

static var EOVERFLOW: POSIXErrorCode

Value too large to be stored in data type.

static var EOWNERDEAD: POSIXErrorCode

Previous owner died.

static var EPERM: POSIXErrorCode

static var EPFNOSUPPORT: POSIXErrorCode

Protocol family not supported.

static var EPIPE: POSIXErrorCode

Broken pipe.

static var EPROCLIM: POSIXErrorCode

quotas & mush. Too many processes.

static var EPROCUNAVAIL: POSIXErrorCode

Bad procedure for program.

static var EPROGMISMATCH: POSIXErrorCode

Program version wrong.

static var EPROGUNAVAIL: POSIXErrorCode

RPC prog. not avail.

static var EPROTO: POSIXErrorCode

Protocol error.

static var EPROTONOSUPPORT: POSIXErrorCode

Protocol not supported.

static var EPROTOTYPE: POSIXErrorCode

Protocol wrong type for socket.

static var EPWROFF: POSIXErrorCode

Intelligent device errors. Device power is off.

static var EQFULL: POSIXErrorCode

Interface output queue is full.

static var ERANGE: POSIXErrorCode

Result too large.

static var EREMOTE: POSIXErrorCode

Too many levels of remote in path.

static var EROFS: POSIXErrorCode

Read-only file system.

static var ERPCMISMATCH: POSIXErrorCode

RPC version wrong.

static var ESHLIBVERS: POSIXErrorCode

Shared library version mismatch.

static var ESHUTDOWN: POSIXErrorCode

Can’t send after socket shutdown.

static var ESOCKTNOSUPPORT: POSIXErrorCode

Socket type not supported.

static var ESPIPE: POSIXErrorCode

Illegal seek.

static var ESRCH: POSIXErrorCode

No such process.

static var ESTALE: POSIXErrorCode

Network File System. Stale NFS file handle.

static var ETIME: POSIXErrorCode

STREAM ioctl timeout.

static var ETIMEDOUT: POSIXErrorCode

Operation timed out.

static var ETOOMANYREFS: POSIXErrorCode

Too many references: can’t splice.

static var ETXTBSY: POSIXErrorCode

Text file busy.

static var EUSERS: POSIXErrorCode

Too many users.

static var EWOULDBLOCK: POSIXErrorCode

Operation would block.

static var EXDEV: POSIXErrorCode

Cross-device link.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error Codes

struct CocoaError

Describes errors within the Cocoa error domain.

struct MachError

Describes an error in the Mach error domain.

NSError Codes

Error codes in the Cocoa error domain.

