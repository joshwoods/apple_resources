

- Kernel
- Kernel Enumerations
- os_log_type_t
-  OS_LOG_TYPE_DEFAULT 

Enumeration Case

# OS_LOG_TYPE_DEFAULT

Default-level messages are initially stored in memory buffers. Without a configuration change, they are compressed and moved to the data store as memory buffers fill. They remain there until a storage quota is exceeded, at which point, the oldest messages are purged. Use this level to capture information about things that *might* result a failure. Logging a message of this type is equivalent to calling the `os_log` function.

macOS 10.12+

``` source
OS_LOG_TYPE_DEFAULT
```

