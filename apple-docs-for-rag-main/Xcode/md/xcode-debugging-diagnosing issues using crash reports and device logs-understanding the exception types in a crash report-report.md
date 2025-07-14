

- Xcode
- Debugging
- Diagnosing issues using crash reports and device logs
-  Understanding the exception types in a crash report 

# Understanding the exception types in a crash report

Learn what the exception type tells you about why your app crashed.

## Overview

The exception type in a crash report describes how the app terminated. It’s a key piece of information that guides how to investigate the source of the problem.

```
Exception Type: EXC_BAD_ACCESS (SIGSEGV)
```

Crash reports record language exception information separately, including language exceptions thrown by an API or language features in Objective-C or C++.

## Topics

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

EXC_RESOURCE

The operating system stopped the process because the process exceeded a limit on resource consumption, like CPU time or memory.

## See Also

### Crash reports

Adding identifiable symbol names to a crash report

Replace hexadecimal addresses in a crash report with function names and line numbers that correspond to your app’s code.

Identifying the cause of common crashes

Find patterns in crash reports that identify common problems, and investigate the issue based on the pattern.

Analyzing a crash report

Identify clues in a crash report that help you diagnose problems.

Examining the fields in a crash report

Understand the structure of a crash report and the information each field contains.

Interpreting the JSON format of a crash report

Understand the structure and properties of the objects the system includes in the JSON of a crash report.

