

- Xcode
- Debugging
- Diagnosing issues using crash reports and device logs
- Understanding the exception types in a crash report
-  EXC_GUARD 

Article

# EXC_GUARD

The process violated a guarded resource protection, often related to file descriptors.

## Overview

There are multiple types of guarded system resources, however most guarded resource crashes are from guarded file descriptors, which have the `GUARD_TYPE_FD` value in the `Exception Subtype` field. The operating system marks a file descriptor as guarded so that normal file descriptor APIs can’t modify them. For example, if an app closes the file descriptor used to access the SQLite file backing a Core Data store, Core Data could mysteriously crash much later on. The guard file description identifies these problems when they happen, making them easier to identify and address.

The `Exception Message` field contains the specific violation:

`CLOSE`  
The process attempted to invoke `close()` on a guarded file descriptor.

`DUP`  
The process attempted to invoke `dup()`, `dup2()`, or `fcntl()` with the `F_DUPFD` or `F_DUPFD_CLOEXEC` commands on a guarded file descriptor.

`NOCLOEXEC`  
The process attempted to remove the `FD_CLOEXEC` flag from a guarded file descriptor.

`SOCKET_IPC`  
The process attempted to send a guarded file descriptor through a socket.

`FILEPORT`  
The process attempted to obtain a Mach send right for a guarded file descriptor.

`WRITE`  
The process attempted to write to a guarded file descriptor.

The `Exception Message` field also identifies the specific guarded file descriptor that the process attempted to modify. To understand the context triggering this exception, consult the backtrace of the crashed thread.

## See Also

### Exceptions

EXC_ARITHMETIC

An arithmetic problem terminated the process, often because of division by zero or a floating-point error.

EXC_BAD_ACCESS

A bad access to memory terminated the process.

EXC_BAD_ACCESS (SIGBUS)

A bus error terminated the process, often because the process tried to access a misaligned or invalid address in memory, or due to a pointer authentication failure.

EXC_BAD_ACCESS (SIGSEGV)

A memory segmentation fault terminated the process, often because the process tried to access an invalid or out-of-bounds address in memory.

EXC_BREAKPOINT (SIGTRAP) and EXC_BAD_INSTRUCTION (SIGILL)

A trace trap or invalid CPU instruction interrupted the process, often because the process violated a requirement or timeout.

EXC_CRASH

The process crashed.

EXC_CRASH (SIGABRT)

The process terminated because it received an abort signal.

EXC_CRASH (SIGKILL)

The operating system terminated the process, often because a background task violated a requirement, device resources were limited, or the user force quit the app.

EXC_CRASH (SIGQUIT)

Another processes terminated the process, often because the process violated a requirement or timeout.

EXC_CRASH (SIGSYS)

A bad argument to a system call terminated the process.

EXC_CRASH (SIGTERM)

A software termination signal terminated the process.

EXC_RESOURCE

The operating system stopped the process because the process exceeded a limit on resource consumption, like CPU time or memory.

