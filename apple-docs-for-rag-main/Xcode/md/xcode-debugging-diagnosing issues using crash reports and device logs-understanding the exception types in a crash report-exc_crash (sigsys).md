

- Xcode
- Debugging
- Diagnosing issues using crash reports and device logs
- Understanding the exception types in a crash report
-  EXC_CRASH (SIGSYS) 

Article

# EXC_CRASH (SIGSYS)

A bad argument to a system call terminated the process.

## Overview

System calls are low-level interfaces that ask the operating system to perform an action. This signal indicates that the requested system call doesn’t exist.

For example, the code below uses system call number 12345, which isn’t valid and produces a `SIGSYS` signal.

```
```

For a list of valid system calls, see the `syscall.h` header file.

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

EXC_CRASH (SIGTERM)

A software termination signal terminated the process.

EXC_GUARD

The process violated a guarded resource protection, often related to file descriptors.

EXC_RESOURCE

The operating system stopped the process because the process exceeded a limit on resource consumption, like CPU time or memory.

