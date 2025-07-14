

- Kernel
- Kernel Enumerations
- os_log_type_t
-  OS_LOG_TYPE_ERROR 

Enumeration Case

# OS_LOG_TYPE_ERROR

Error-level messages are always saved in the data store. They remain there until a storage quota is exceeded, at which point, the oldest messages are purged. Error-level messages are intended for reporting process-level errors. If an activity object exists, logging at this level captures information for the entire process chain. Logging a message of this type is equivalent to calling the `os_log_error` function.

macOS 10.12+

``` source
OS_LOG_TYPE_ERROR
```

