

- System
-  Adopting Swift Error Constants 

Article

# Adopting Swift Error Constants

Migrate existing C code to Swift, using the error constants provided by the System module.

## Overview

The C error constants map to Swift as follows:

- `E2BIG` ⟶ argListTooLong

- `EACCES` ⟶ permissionDenied

- `EADDRINUSE` ⟶ addressInUse

- `EADDRNOTAVAIL` ⟶ addressNotAvailable

- `EAFNOSUPPORT` ⟶ addressFamilyNotSupported

- `EAGAIN` ⟶ resourceTemporarilyUnavailable

- `EALREADY` ⟶ alreadyInProcess

- `EAUTH` ⟶ authenticationError

- `EBADARCH` ⟶ badCPUType

- `EBADEXEC` ⟶ badExecutable

- `EBADF` ⟶ badFileDescriptor

- `EBADMACHO` ⟶ malformedMachO

- `EBADMSG` ⟶ badMessage

- `EBADRPC` ⟶ rpcUnsuccessful

- `EBUSY` ⟶ resourceBusy

- `ECANCELED` ⟶ canceled

- `ECHILD` ⟶ noChildProcess

- `ECONNABORTED` ⟶ connectionAbort

- `ECONNREFUSED` ⟶ connectionRefused

- `ECONNRESET` ⟶ connectionReset

- `EDEADLK` ⟶ deadlock

- `EDESTADDRREQ` ⟶ addressRequired

- `EDEVERR` ⟶ deviceError

- `EDOM` ⟶ outOfDomain

- `EDQUOT` ⟶ diskQuotaExceeded

- `EEXIST` ⟶ fileExists

- `EFAULT` ⟶ badAddress

- `EFBIG` ⟶ fileTooLarge

- `EFTYPE` ⟶ badFileTypeOrFormat

- `EHOSTDOWN` ⟶ hostIsDown

- `EHOSTUNREACH` ⟶ noRouteToHost

- `EIDRM` ⟶ identifierRemoved

- `EILSEQ` ⟶ illegalByteSequence

- `EINPROGRESS` ⟶ nowInProgress

- `EINTR` ⟶ interrupted

- `EINVAL` ⟶ invalidArgument

- `EIO` ⟶ ioError

- `EISCONN` ⟶ socketIsConnected

- `EISDIR` ⟶ isDirectory

- `ELAST` ⟶ lastErrnoValue

- `ELOOP` ⟶ tooManySymbolicLinkLevels

- `EMFILE` ⟶ tooManyOpenFiles

- `EMLINK` ⟶ tooManyLinks

- `EMSGSIZE` ⟶ messageTooLong

- `EMULTIHOP` ⟶ multiHop

- `ENAMETOOLONG` ⟶ fileNameTooLong

- `ENEEDAUTH` ⟶ needAuthenticator

- `ENETDOWN` ⟶ networkDown

- `ENETRESET` ⟶ networkReset

- `ENETUNREACH` ⟶ networkUnreachable

- `ENFILE` ⟶ tooManyOpenFilesInSystem

- `ENOATTR` ⟶ attributeNotFound

- `ENOBUFS` ⟶ noBufferSpace

- `ENODATA` ⟶ noData

- `ENODEV` ⟶ operationNotSupportedByDevice

- `ENOENT` ⟶ noSuchFileOrDirectory

- `ENOEXEC` ⟶ execFormatError

- `ENOLCK` ⟶ noLocks

- `ENOLINK` ⟶ noLink

- `ENOMEM` ⟶ noMemory

- `ENOMSG` ⟶ noMessage

- `ENOPOLICY` ⟶ noSuchPolicy

- `ENOPROTOOPT` ⟶ protocolNotAvailable

- `ENOSPC` ⟶ noSpace

- `ENOSR` ⟶ noStreamResources

- `ENOSTR` ⟶ notStream

- `ENOSYS` ⟶ noFunction

- `ENOTBLK` ⟶ notBlockDevice

- `ENOTCONN` ⟶ socketNotConnected

- `ENOTDIR` ⟶ notDirectory

- `ENOTEMPTY` ⟶ directoryNotEmpty

- `ENOTRECOVERABLE` ⟶ notRecoverable

- `ENOTSOCK` ⟶ notSocket

- `ENOTSUP` ⟶ notSupported

- `ENOTTY` ⟶ inappropriateIOCTLForDevice

- `ENXIO` ⟶ noSuchAddressOrDevice

- `EOPNOTSUPP` ⟶ notSupportedOnSocket

- `EOVERFLOW` ⟶ overflow

- `EOWNERDEAD` ⟶ previousOwnerDied

- `EPERM` ⟶ notPermitted

- `EPFNOSUPPORT` ⟶ protocolFamilyNotSupported

- `EPIPE` ⟶ brokenPipe

- `EPROCLIM` ⟶ tooManyProcesses

- `EPROCUNAVAIL` ⟶ rpcProcedureUnavailable

- `EPROGMISMATCH` ⟶ rpcProgramVersionMismatch

- `EPROGUNAVAIL` ⟶ rpcProgramUnavailable

- `EPROTONOSUPPORT` ⟶ protocolNotSupported

- `EPROTOTYPE` ⟶ protocolWrongTypeForSocket

- `EPROTO` ⟶ protocolError

- `EPWROFF` ⟶ devicePowerIsOff

- `EQFULL` ⟶ outputQueueFull

- `ERANGE` ⟶ outOfRange

- `EREMOTE` ⟶ tooManyRemoteLevels

- `EROFS` ⟶ readOnlyFileSystem

- `ERPCMISMATCH` ⟶ rpcVersionMismatch

- `ESHLIBVERS` ⟶ sharedLibraryVersionMismatch

- `ESHUTDOWN` ⟶ socketShutdown

- `ESOCKTNOSUPPORT` ⟶ socketTypeNotSupported

- `ESPIPE` ⟶ illegalSeek

- `ESRCH` ⟶ noSuchProcess

- `ESTALE` ⟶ staleNFSFileHandle

- `ETIMEDOUT` ⟶ timedOut

- `ETIME` ⟶ timeout

- `ETOOMANYREFS` ⟶ tooManyReferences

- `ETXTBSY` ⟶ textFileBusy

- `EUSERS` ⟶ tooManyUsers

- `EWOULDBLOCK` ⟶ wouldBlock

- `EXDEV` ⟶ improperLink

## See Also

### Adopting System

Adopting Swift File Operations

Migrate existing C code to Swift, using the file operations provided by the System module.

Adopting Swift File Options

Migrate existing C code to Swift, using the file-operation options provided by the System module.

