

- Kernel
- Deprecated Symbols
-  IOHIDEventService Deprecated

Class

# IOHIDEventService

IOService represents an device or OS service in IOKit and DriverKit.

macOS 10.12.2–10.15.2Deprecated

``` source
class IOHIDEventService : IOService
```

## Overview

IOKit provides driver lifecycle management through the IOService APIs. Drivers and devices are represented as subclasses of IOService.

## Topics

### Miscellaneous

dispatchDigitizerEvent

Dispatch tablet events without orientation

dispatchDigitizerEventWithPolarOrientation

Dispatch tablet events with polar orientation

dispatchDigitizerEventWithTiltOrientation

Dispatch tablet events with tilt orientation

dispatchMultiAxisPointerEvent

Dispatch multi-axis pointer event

handleClose

Handle a client close on the interface.

handleIsOpen

Query whether a client has an open on the interface.

handleOpen

Handle a client open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

handleStop

Quiesce the hardware and stop the driver.

### Instance Variables

_reserved

### Instance Methods

- CopyEvent

- CreateAction_CopyEvent

- CreateAction_SetLED

- CreateAction_SetUserProperties

- Dispatch

- EventAvailable

- EventAvailable_Impl

- SetEventMemory

- SetEventMemory_Impl

- SetLED

- SetLEDAction

- SetLEDState

- SetLEDState_Impl

- SetLED_Impl

- SetProperties_Impl

- SetUserProperties

- Start_Impl

- Stop_Impl

- calculateStandardType

- close

- closeForClient

- completeCopyEvent

- completeSetLED

- completeSetProperties

- copyEvent

- copyEventForClient

- copyMatchingEvent

- copyPropertyForClient

- determineResolution

- dispatchAbsolutePointerEvent

- dispatchBiometricEvent

- dispatchDigitizerEvent

- dispatchDigitizerEventWithOrientation

- dispatchDigitizerEventWithPolarOrientation

- dispatchDigitizerEventWithTiltOrientation

- dispatchEvent

Dispatches an event.

- dispatchExtendedGameControllerEvent

- dispatchExtendedGameControllerEventWithOptionalBottomButtons

- dispatchExtendedGameControllerEventWithOptionalButtons

- dispatchExtendedGameControllerEventWithThumbstickButtons

- dispatchKeyboardEvent

- dispatchKeyboardEvent

- dispatchMultiAxisPointerEvent

- dispatchRelativePointerEvent

- dispatchRelativePointerEventWithFixed

- dispatchScrollWheelEvent

- dispatchScrollWheelEventWithFixed

- dispatchStandardGameControllerEvent

- dispatchTabletPointerEvent

- dispatchTabletProximityEvent

- dispatchUnicodeEvent

- free

- getCountryCode

- getDeviceUsagePairs

- getElementValue

- getLocationID

- getManufacturer

- getMetaClass

- getPrimaryUsage

- getPrimaryUsagePage

- getProduct

- getProductID

- getReportElements

- getReportInterval

- getSerialNumber

- getTransport

- getVendorID

- getVendorIDSource

- getVersion

- handleClose

- handleCopyMatchingEvent

- handleCopyMatchingEvent_Impl

- handleIsOpen

- handleOpen

- handleStart

- handleStop

- init

- isPowerButtonNmiEnabled

- matchPropertyTable

- message

- multiAxisTimerCallback

- newConsumerShim

- newKeyboardShim

- newUserClient

- open

- openForClient

- parseSupportedElements

- processTabletElement

- readyForReports

- setElementValue

- setProperties

- setPropertiesForClient

- setSystemProperties

- start

- stop

- supportsHeadset

### Type Methods

+ CopyEvent_Invoke

+ CopyEvent_Invoke

+ EventAvailable_Invoke

+ SetEventMemory_Invoke

+ SetLEDAction_Invoke

+ SetLEDAction_Invoke

+ SetLEDState_Invoke

+ SetLED_Invoke

+ SetUserProperties_Invoke

+ SetUserProperties_Invoke

+ debugActionNMI

+ debugActionSysdiagnose

+ handleCopyMatchingEvent_Invoke

+ powerButtonNMI

## Relationships

### Inherits From

- IOService

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

IOUSBHostPipeDeprecated

IOUSBHostIOSourceDeprecated

IOUSBHostStreamDeprecated

IOHIDEventDriverDeprecated

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

