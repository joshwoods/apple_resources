

- CFNetwork
- CFHostClientContext
-  copyDescription 

Instance Property

# copyDescription

The callback used to create a descriptive string representation of the info pointer (or the data pointed to by the info pointer) for debugging purposes. This callback is called by the CFCopyDescription(_:) function.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var copyDescription: CFAllocatorCopyDescriptionCallBack?
```

## See Also

### Instance Properties

var info: UnsafeMutableRawPointer?

An arbitrary pointer to allocated memory containing user-defined data that can be associated with the host and that is passed to the callbacks.

var release: CFAllocatorReleaseCallBack?

The callback used to remove a retain previously added for the host on the info pointer.

var retain: CFAllocatorRetainCallBack?

The callback used to add a retain for the host on the info pointer for the life of the host, and may be used for temporary references the host needs to take. This callback returns the actual info pointer to store in the host, almost always just the pointer passed as the parameter.

var version: CFIndex

The version number of the structure type passed as a parameter to the host client function. The only valid version number is `0`.

