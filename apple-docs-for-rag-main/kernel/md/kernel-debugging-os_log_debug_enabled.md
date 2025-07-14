

- Kernel
- Debugging
-  os_log_debug_enabled 

Function

# os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

macOS 10.12+

``` source
bool os_log_debug_enabled(os_log_t log);
```

## Parameters 

`log`  

The `OS_LOG_DEFAULT` constant or a custom log object previously created by the os_log_create function.

## Return Value

`YES` if debug-level logging is enabled, otherwise `NO`.

## See Also

### Logging

OS_os_log

IOLog

Log a message to console in text mode, and /var/log/system.log.

IOLogv

Log a message to console in text mode, and /var/log/system.log.

os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

### Related Documentation

isEnabled(type:)

Returns a Boolean value that indicates whether the log can write messages with the specified log type.

OS_LOG_TYPE_DEBUG

Debug-level messages are only captured in memory when debug logging is enabled through a configuration change. They’re purged in accordance with the configuration’s persistence setting. Messages logged at this level contain information that may be useful during development or while troubleshooting a specific problem. Debug logging is intended for use in a development environment and not in shipping software. Logging a message of this type is equivalent to calling the function.

