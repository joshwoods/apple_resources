

- Xcode
- Debugging
- Diagnosing issues using crash reports and device logs
- Understanding the exception types in a crash report
-  EXC_RESOURCE 

Article

# EXC_RESOURCE

The operating system stopped the process because the process exceeded a limit on resource consumption, like CPU time or memory.

## Overview

If the `Exception Note` field contains `NON-FATAL CONDITION`, this means the operating system generated a crash report without actually terminating the process. The `Exception Message` field describes the amount of resources consumed over a specific time interval.

The crash report lists the specific resource in the `Exception Subtype` field:

`CPU` and `CPU_FATAL`  
A thread in the process used too much CPU over a short period of time.

`MEMORY`  
The process crossed a memory limit imposed by the system. This may be a precursor to termination for excess memory usage.

`IO`  
The process caused an excessive amount of disk writes over a short period of time.

`WAKEUPS`  
Threads in the process woke up too many times per second, which consumes battery life.

Excessive wake-ups can come from calling thread-to-thread communication APIs more often than expected; these APIs include perform(_:on:with:waitUntilDone:), async(execute:), and dispatch_async. Because the communication that triggers this exception is happening so frequently, crash reports usually include multiple background threads with very similar backtraces that indicate the origin of the thread communication. See Modernizing Grand Central Dispatch Usage for how to manage concurrent workloads more efficiently.

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

EXC_GUARD

The process violated a guarded resource protection, often related to file descriptors.

