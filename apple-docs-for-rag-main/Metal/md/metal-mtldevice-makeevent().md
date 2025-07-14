

- Metal
- MTLDevice
-  makeEvent() 

Instance Method

# makeEvent()

Creates a new event instance that you can use to synchronize commands and resources within the same GPU device.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func makeEvent() -> (any MTLEvent)?
```

**Required**

## See Also

### Creating Fences and Events

func makeFence() -> (any MTLFence)?

Creates a new memory fence instance.

**Required**

func makeSharedEvent() -> (any MTLSharedEvent)?

Creates a new shared event instance that you can use to synchronize commands and resources across different GPU devices.

**Required**

func makeSharedEvent(handle: MTLSharedEventHandle) -> (any MTLSharedEvent)?

Recreates a shared event from a handle.

**Required**

