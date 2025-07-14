

- Metal
- MTLDevice
-  makeFence() 

Instance Method

# makeFence()

Creates a new memory fence instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func makeFence() -> (any MTLFence)?
```

**Required**

## See Also

### Creating Fences and Events

func makeEvent() -> (any MTLEvent)?

Creates a new event instance that you can use to synchronize commands and resources within the same GPU device.

**Required**

func makeSharedEvent() -> (any MTLSharedEvent)?

Creates a new shared event instance that you can use to synchronize commands and resources across different GPU devices.

**Required**

func makeSharedEvent(handle: MTLSharedEventHandle) -> (any MTLSharedEvent)?

Recreates a shared event from a handle.

**Required**

