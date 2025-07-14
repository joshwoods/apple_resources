

- Kernel
- Debugging
-  IOLog 

Function

# IOLog

Log a message to console in text mode, and /var/log/system.log.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
int IOLog(const char *format, ...);
```

**macOS**

``` source
void IOLog(const char *format, ...);
```

## Parameters 

`format`  

A printf() style format string (see printf(3) documentation).

`other`  

arguments described by the format string.

## Discussion

This function allows a driver to log diagnostic information to the screen during verbose boots, and to a log file found at /var/log/system.log. IOLog should not be called from interrupt context.

## See Also

### Logging

OS_os_log

IOLogv

Log a message to console in text mode, and /var/log/system.log.

os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

