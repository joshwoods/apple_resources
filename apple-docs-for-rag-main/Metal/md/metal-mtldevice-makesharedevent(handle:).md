

- Metal
- MTLDevice
-  makeSharedEvent(handle:) 

Instance Method

# makeSharedEvent(handle:)

Recreates a shared event from a handle.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func makeSharedEvent(handle sharedEventHandle: MTLSharedEventHandle) -> (any MTLSharedEvent)?
```

**Required**

## Parameters 

`sharedEventHandle`  

An MTLSharedEventHandle instance from another GPU device or process.

## Return Value

A new MTLSharedEvent instance if the method completed successfully; otherwise nil.

## See Also

### Creating Fences and Events

func makeFence() -> (any MTLFence)?

Creates a new memory fence instance.

**Required**

func makeEvent() -> (any MTLEvent)?

Creates a new event instance that you can use to synchronize commands and resources within the same GPU device.

**Required**

func makeSharedEvent() -> (any MTLSharedEvent)?

Creates a new shared event instance that you can use to synchronize commands and resources across different GPU devices.

**Required**

