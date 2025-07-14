

- Core Services
- Carbon Core
- Carbon Core Structures
-  FSEventStreamContext 

Structure

# FSEventStreamContext

Mac Catalyst 13.0+macOS 10.5+

``` source
struct FSEventStreamContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: CFAllocatorRetainCallBack?, release: CFAllocatorReleaseCallBack?, copyDescription: CFAllocatorCopyDescriptionCallBack?)

### Instance Properties

var copyDescription: CFAllocatorCopyDescriptionCallBack?

The callback used to create a descriptive string representation of the info pointer (or the data pointed to by the info pointer) for debugging purposes. This can be NULL.

var info: UnsafeMutableRawPointer?

An arbitrary client-defined value (for instance, a pointer) to be associated with the stream and passed to the callback when it is invoked. If a non-NULL value is supplied for the retain callback the framework will use it to retain this value. If a non-NULL value is supplied for the release callback then when the stream is deallocated it will be used to release this value. This can be NULL.

var release: CFAllocatorReleaseCallBack?

The callback used release a retain on the info pointer. This can be NULL.

var retain: CFAllocatorRetainCallBack?

The callback used retain the info pointer. This can be NULL.

var version: CFIndex

Currently the only valid value is zero.

