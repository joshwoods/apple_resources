

- Core Services
- Carbon Core
- Carbon Core Structures
- FSEventStreamContext
-  info 

Instance Property

# info

An arbitrary client-defined value (for instance, a pointer) to be associated with the stream and passed to the callback when it is invoked. If a non-NULL value is supplied for the retain callback the framework will use it to retain this value. If a non-NULL value is supplied for the release callback then when the stream is deallocated it will be used to release this value. This can be NULL.

Mac Catalyst 13.0+macOS 10.5+

``` source
var info: UnsafeMutableRawPointer?
```

