

- Kernel
- Deprecated Symbols
-  IOUSBHostDevice Deprecated

Class

# IOUSBHostDevice

macOS 10.11–10.15.4Deprecated

``` source
class IOUSBHostDevice : IOUSBDevice
```

## Topics

### Instance Methods

- AbortDeviceRequests

- AbortDeviceRequests_Impl

- AsyncDeviceRequest

- AsyncDeviceRequest_Impl

- Close

- Close_Impl

- CompleteAsyncDeviceRequest

- CopyInterface

- CopyInterface_Impl

- CreateIOBuffer

- CreateIOBuffer_Impl

- CreateInterfaceIterator

- CreateInterfaceIterator_Impl

- DestroyInterfaceIterator

- DestroyInterfaceIterator_Impl

- DeviceRequest

- DeviceRequest_Impl

- Dispatch

- GetAddress

- GetAddress_Impl

- GetFrameNumber

- GetFrameNumber_Impl

- GetPortStatus

- GetPortStatus_Impl

- GetSpeed

- GetSpeed_Impl

- Open

- Open_Impl

- PMstop

- Reset

- Reset_Impl

- SetConfiguration

- SetConfiguration_Impl

- abortDeviceRequests

- abortDeviceRequestsGated

- addPowerChild

- addPowerChildGated

- addPowerChildThreadCall

- allocateDownstreamBusCurrent

- allocateDownstreamBusCurrentGated

- attach

- cacheDescriptor

- cacheDescriptorGated

- close

- closeGated

- compareProperty

- compareProperty

- createIOBuffer

- createPipe

- createPipeGated

- deviceRequest

- deviceRequest

- deviceRequest

- deviceRequest

- deviceRequest

- forcePower

- forcePowerGated

- free

- getAddress

- getCapabilityDescriptors

- getConfigurationDescriptor

- getConfigurationDescriptor

- getConfigurationDescriptorWithValue

- getDescriptor

- getDescriptorGated

- getDeviceDescriptor

- getFrameNumber

- getLPMExitLatency

- getLPMExitLatencyGated

- getMetaClass

- getPortStatus

- getSpeed

- getStringDescriptor

- handleClose

- handleIsOpen

- handleOpen

- idleAssertion

- initWithController

- initialPowerStateForDomainState

- internalDeviceRequest

- internalDeviceRequestGated

- matchPropertyTable

- matchPropertyTable

- message

- newUserClient

- open

- openGated

- pmStopThreadCall

- powerChangeDone

- powerStateDidChangeTo

- powerStateDidChangeToGated

- powerStateWillChangeTo

- powerStateWillChangeToGated

- registerPowerService

- removePowerChild

- reset

- setConfiguration

- setConfigurationGated

- setPowerState

- setPowerStateGated

- setProperties

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- setProperty

- start

- stop

- stringFromReturn

- terminate

- terminateGated

- updateIdlePolicy

- updateIdlePolicyAsync

- updateIdlePolicyGated

- updateLPMPolicyGated

### Type Methods

+ AbortDeviceRequests_Invoke

+ AsyncDeviceRequest_Invoke

+ Close_Invoke

+ CompleteAsyncDeviceRequest_Invoke

+ CompleteAsyncDeviceRequest_Invoke

+ CopyInterface_Invoke

+ CreateIOBuffer_Invoke

+ CreateInterfaceIterator_Invoke

+ DestroyInterfaceIterator_Invoke

+ DeviceRequest_Invoke

+ GetAddress_Invoke

+ GetFrameNumber_Invoke

+ GetPortStatus_Invoke

+ GetSpeed_Invoke

+ Open_Invoke

+ Reset_Invoke

+ SetConfiguration_Invoke

+ asyncDeviceRequestCompletionCallback

+ withController

## Relationships

### Inherits From

- IOUSBDevice

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

IOUSBHostPipeDeprecated

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

