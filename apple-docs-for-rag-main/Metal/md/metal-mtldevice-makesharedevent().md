

- Metal
- MTLDevice
-  makeSharedEvent() 

Instance Method

# makeSharedEvent()

Creates a new shared event instance that you can use to synchronize commands and resources across different GPU devices.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func makeSharedEvent() -> (any MTLSharedEvent)?
```

**Required**

## See Also

### Creating Fences and Events

func makeFence() -> (any MTLFence)?

Creates a new memory fence instance.

**Required**

func makeEvent() -> (any MTLEvent)?

Creates a new event instance that you can use to synchronize commands and resources within the same GPU device.

**Required**

func makeSharedEvent(handle: MTLSharedEventHandle) -> (any MTLSharedEvent)?

Recreates a shared event from a handle.

**Required**

