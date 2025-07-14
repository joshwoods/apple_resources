

- Kernel
- Deprecated Symbols
-  IOHIDInterface Deprecated

Class

# IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

macOS 10.4–10.15.2Deprecated

``` source
class IOHIDInterface : IOService
```

## Overview

IOKit provides driver lifecycle management through the IOService APIs. Drivers and devices are represented as subclasses of IOService.

## Topics

### Miscellaneous

free

Free the IOHIDInterface object.

init

Initialize an IOHIDInterface object.

matchPropertyTable

Called by the provider during a match

start

Start up the driver using the given provider.

### Callbacks

CompletionAction

InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

IOHIDInterface::CompletionAction

IOHIDInterface::InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

### Instance Variables

_reserved

### Instance Methods

- AddReportToPool

- AddReportToPool_Impl

- Close

- Close_Impl

- Dispatch

- GetElementValues

- GetElementValues_Impl

- GetReport

- GetReport_Impl

- GetSupportedCookies

- GetSupportedCookies_Impl

- HandleReportPrivate

- Open

- Open_Impl

- ReportAvailable

- SendDebugBuffer

- SendDebugBuffer_Impl

- SetElementValues

- SetElementValues_Impl

- SetReport

- SetReport_Impl

- addReportToPoolGated

- close

- createElements

- createMatchingElements

- free

- getCountryCode

- getLocationID

- getManufacturer

- getMaxReportSize

- getMetaClass

- getProduct

- getProductID

- getReport

- getReport

- getReportInterval

- getSerialNumber

- getTransport

- getVendorID

- getVendorIDSource

- getVersion

- handleReport

- handleReportGated

- init

Initializes IOHIDInterface object.

- matchPropertyTable

- message

- open

- openGated

- serializeDebugState

- setProperty

- setReport

- setReport

- start

- stop

### Type Methods

+ AddReportToPool_Invoke

+ Close_Invoke

+ GetElementValues_Invoke

+ GetReport_Invoke

+ GetSupportedCookies_Invoke

+ Open_Invoke

+ ReportAvailable_Invoke

+ ReportAvailable_Invoke

+ SendDebugBuffer_Invoke

+ SetElementValues_Invoke

+ SetReport_Invoke

+ withElements

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

IOHIDEventService

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

