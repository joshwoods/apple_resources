

- Kernel
- Kernel Enumerations
- os_log_type_t
-  OS_LOG_TYPE_INFO 

Enumeration Case

# OS_LOG_TYPE_INFO

Info-level messages are initially stored in memory buffers. Without a configuration change, they are not moved to the data store and are purged as memory buffers fill. They are, however, captured in the data store when faults and, optionally, errors occur. When info-level messages are added to the data store, they remain there until a storage quota is exceeded, at which point, the oldest messages are purged. Use this level to capture information that may be helpful, but isn’t essential, for troubleshooting errors. Logging a message of this type is equivalent to calling the `os_log_info` function.

macOS 10.12+

``` source
OS_LOG_TYPE_INFO
```

