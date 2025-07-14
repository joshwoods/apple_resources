

- Kernel
- Debugging
-  IOLogv 

Function

# IOLogv

Log a message to console in text mode, and /var/log/system.log.

DriverKitKernelDriverKit 24.4+macOS 10.6+

**DriverKit**

``` source
int IOLogv(const char *format, va_list ap);
```

**macOS**

``` source
void IOLogv(const char *format, va_list ap);
```

## Parameters 

`format`  

A printf() style format string (see printf(3) documentation).

`ap`  

stdarg(3) style variable arguments.

## Discussion

This function allows a driver to log diagnostic information to the screen during verbose boots, and to a log file found at /var/log/system.log. IOLogv should not be called from interrupt context.

## See Also

### Logging

OS_os_log

IOLog

Log a message to console in text mode, and /var/log/system.log.

os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

