

- Kernel
- Debugging
-  os_log_create 

Function

# os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

macOS 10.12+

``` source
os_log_t os_log_create(const char *subsystem, const char *category);
```

## Parameters 

`subsystem`  

An identifier string, in reverse DNS notation, representing the subsystem that’s performing logging. For example, `com.your_company.your_subsystem_name`. The subsystem is used for categorization and filtering of related log messages, as well as for grouping related logging settings.

`category`  

A category within the specified subsystem. The category is used for categorization and filtering of related log messages, as well as for grouping related logging settings within the subsystem’s settings. A category’s logging settings override those of the parent subsystem.

## Return Value

A value of type `os_log_t`, which can be passed to other logging functions to perform logging and to determine whether a specific level of logging is enabled. A value is always returned and should be released when no longer needed.

## Discussion

Generally, use the `OS_LOG_DEFAULT` constant to perform logging using the system’s behavior. Create a custom log object only when you want to tag messages with a specific subsystem and category for the purpose of filtering, or to customize the logging behavior of your subsystem with a profile for debugging purposes. This function only needs to be called once to initialize a custom log object. It doesn’t need to be called again when changing logging settings. The system automatically detects changes to logging settings.

## See Also

### Logging

OS_os_log

IOLog

Log a message to console in text mode, and /var/log/system.log.

IOLogv

Log a message to console in text mode, and /var/log/system.log.

os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

### Related Documentation

OS_LOG_TYPE_DEFAULT

Default-level messages are initially stored in memory buffers. Without a configuration change, they are compressed and moved to the data store as memory buffers fill. They remain there until a storage quota is exceeded, at which point, the oldest messages are purged. Use this level to capture information about things that *might* result a failure. Logging a message of this type is equivalent to calling the function.

isEnabled(type:)

Returns a Boolean value that indicates whether the log can write messages with the specified log type.

