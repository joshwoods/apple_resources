

- Kernel
- Debugging
-  os_log_info_enabled 

Function

# os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

macOS 10.12+

``` source
bool os_log_info_enabled(os_log_t log);
```

## Parameters 

`log`  

The `OS_LOG_DEFAULT` constant or a custom log object previously created by the os_log_create function.

## Return Value

`YES` if info-level logging is enabled, otherwise `NO`.

## See Also

### Logging

OS_os_log

IOLog

Log a message to console in text mode, and /var/log/system.log.

IOLogv

Log a message to console in text mode, and /var/log/system.log.

os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

### Related Documentation

OS_LOG_TYPE_INFO

Info-level messages are initially stored in memory buffers. Without a configuration change, they are not moved to the data store and are purged as memory buffers fill. They are, however, captured in the data store when faults and, optionally, errors occur. When info-level messages are added to the data store, they remain there until a storage quota is exceeded, at which point, the oldest messages are purged. Use this level to capture information that may be helpful, but isn’t essential, for troubleshooting errors. Logging a message of this type is equivalent to calling the function.

isEnabled(type:)

Returns a Boolean value that indicates whether the log can write messages with the specified log type.

