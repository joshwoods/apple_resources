

- CFNetwork
- CFHostClientContext
-  init(version:info:retain:release:copyDescription:) 

Initializer

# init(version:info:retain:release:copyDescription:)

Initializes an object that contains user-defined data and callbacks for a network host using the specified values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer?,
    retain: CFAllocatorRetainCallBack?,
    release: CFAllocatorReleaseCallBack?,
    copyDescription: CFAllocatorCopyDescriptionCallBack?
)
```

## See Also

### Initializers

init()

Initializes an object that contains user-defined data and callbacks for a network host.

