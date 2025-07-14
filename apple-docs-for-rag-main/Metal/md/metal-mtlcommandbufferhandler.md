

- Metal
-  MTLCommandBufferHandler 

Type Alias

# MTLCommandBufferHandler

A completion handler signature a GPU device calls when it finishes scheduling a command buffer, or when the GPU finishes running it.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLCommandBufferHandler = (any MTLCommandBuffer) -> Void
```

## Parameters 

`commandBuffer`  

The MTLCommandBuffer instance that’s invoking the completion handler.

## Discussion

The MTLCommandBuffer type uses this signature in its methods that register your completion handlers, including addScheduledHandler(_:) and addCompletedHandler(_:).

## See Also

### Registering State Change Handlers

func addScheduledHandler(MTLCommandBufferHandler)

Registers a completion handler the GPU device calls immediately after it schedules the command buffer to run on the GPU.

**Required**

func addCompletedHandler(MTLCommandBufferHandler)

Registers a completion handler the GPU device calls immediately after the GPU finishes running the commands in the command buffer.

**Required**

