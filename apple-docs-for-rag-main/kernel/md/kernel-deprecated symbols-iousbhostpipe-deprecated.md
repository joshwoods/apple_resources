

- Kernel
- Deprecated Symbols
-  IOUSBHostPipe Deprecated

Class

# IOUSBHostPipe

macOS 10.11–10.15.4Deprecated

``` source
class IOUSBHostPipe : IOUSBHostIOSource
```

## Topics

### Instance Methods

- Abort

- Abort_Impl

- AdjustPipe

- AdjustPipe_Impl

- AsyncIO

- AsyncIOBundled

- AsyncIOBundled_Impl

- AsyncIO_Impl

- ClearStall

- ClearStall_Impl

- CompleteAsyncIO

- CompleteAsyncIOBundled

- CompleteAsyncIsochIO

- CreateMemoryDescriptorRing

- CreateMemoryDescriptorRing_Impl

- Dispatch

- GetDescriptors

- GetDescriptors_Impl

- GetDeviceAddress

- GetDeviceAddress_Impl

- GetIdlePolicy

- GetIdlePolicy_Impl

- GetSpeed

- GetSpeed_Impl

- IO

- IO_Impl

- IsochIO

- IsochIO_Impl

- SetIdlePolicy

- SetIdlePolicy_Impl

- SetMemoryDescriptor

- SetMemoryDescriptor_Impl

- abort

- abortGated

- adjustOutstandingIO

- adjustPipe

- adjustPipe

- adjustPipeGated

- adjustPipeGatedV2

- clearStall

- clearStallGated

- closeGated

- controlRequest

- controlRequest

- controlRequest

- controlRequest

- controlRequestGated

- copyStream

- copyStreamGated

- destroyGated

- destroyMemoryDescriptorRing

- disableStreams

- disableStreamsGated

- enableStreams

- enableStreamsGated

- free

- getDescriptors

- getDeviceAddress

- getEndpointDescriptor

- getIdlePolicy

- getIdlePolicyGated

- getMetaClass

- getOutstandingIO

- getSpeed

- getSuperSpeedEndpointCompanionDescriptor

- initWithDescriptorsAndOwners

- io

- io

- io

- io

- io

- io

- isochronousIoGated

- openGated

- setIdlePolicy

- setIdlePolicyGated

### Type Methods

+ Abort_Invoke

+ AdjustPipe_Invoke

+ AsyncIOBundled_Invoke

+ AsyncIO_Invoke

+ ClearStall_Invoke

+ CompleteAsyncIOBundled_Invoke

+ CompleteAsyncIOBundled_Invoke

+ CompleteAsyncIO_Invoke

+ CompleteAsyncIO_Invoke

+ CompleteAsyncIsochIO_Invoke

+ CompleteAsyncIsochIO_Invoke

+ CreateMemoryDescriptorRing_Invoke

+ GetDescriptors_Invoke

+ GetDeviceAddress_Invoke

+ GetIdlePolicy_Invoke

+ GetSpeed_Invoke

+ IO_Invoke

+ IsochIO_Invoke

+ SetIdlePolicy_Invoke

+ SetMemoryDescriptor_Invoke

+ asyncIOCompletionCallback

+ asyncIOCompletionCallbackBundled

+ asyncIsochIOCompletionCallback

+ asyncIsochIOTransactionCompletionCallback

+ isochIOTransactionCompatCallback

+ rawBufferControlRequestCompletion

+ withDescriptorsAndOwners

## Relationships

### Inherits From

- IOUSBHostIOSource

## See Also

### IOKit

IOUSBDevice

An input/output service object that represents a device on the USB bus.

Deprecated

IOUSBInterface

An object that represents an interface of a device on the USB bus.

Deprecated

IOOFPathMatchingDeprecated

IOUSBHostInterfaceDeprecated

IOUSBHostDeviceDeprecated

IOUSBHostIOSourceDeprecated

IOUSBHostStreamDeprecated

IOHIDEventDriverDeprecated

IOHIDEventService

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDSystemDeprecated

IOHIKeyboardMapperDeprecated

IOHIKeyboardDeprecated

IOHIPointingDeprecated

IOHIDeviceDeprecated

IOHIDElementDeprecated

IOHIDWorkLoopDeprecated

IOEthernetInterface

The Ethernet interface object.

Deprecated

IOEthernetController

Abstract superclass for Ethernet controllers.

Deprecated

