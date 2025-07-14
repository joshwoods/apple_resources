

- Kernel
- Deprecated Symbols
-  IOHIDEventDriver Deprecated

Class

# IOHIDEventDriver

macOS 10.12.2–10.15.1Deprecated

``` source
class IOHIDEventDriver : IOHIDEventService
```

## Topics

### Instance Methods

- checkGameControllerElement

- checkMultiAxisElement

- conformTo

- copyEvent

- copyMatchingEvent

- createDigitizerTransducerEventForReport

- didTerminate

- dispatchEvent

- free

- getBlessedUsagePairs

- getButtonStateFromElements

- getCountryCode

- getElementValue

- getLocationID

- getManufacturer

- getMetaClass

- getProduct

- getProductID

- getReportElements

- getSerialNumber

- getTransport

- getVendorID

- getVendorIDSource

- getVersion

- handleAccelReport

- handleBiometricReport

- handleBootPointingReport

- handleCompassReport

- handleDeviceOrientationReport

- handleDigitizerCollectionReport

- handleDigitizerReport

- handleDigitizerTransducerReport

- handleGameControllerReport

- handleGyroReport

- handleInterruptReport

- handleKeboardReport

- handleMultiAxisPointerReport

- handlePhaseReport

- handleProximityReport

- handleRelativeReport

- handleScrollReport

- handleStart

- handleStop

- handleTemperatureReport

- handleUnicodeGestureCandidateReport

- handleUnicodeGestureReport

- handleUnicodeLegacyReport

- handleUnicodeReport

- handleVendorMessageReport

- init

- parseAccelElement

- parseBiometricElement

- parseCompassElement

- parseDeviceOrientationElement

- parseDigitizerElement

- parseDigitizerTransducerElement

- parseElements

- parseGameControllerElement

- parseGestureUnicodeElement

- parseGyroElement

- parseKeyboardElement

- parseLEDElement

- parseLegacyUnicodeElement

- parseMultiAxisElement

- parsePhaseElement

- parseProximityElement

- parseRelativeElement

- parseScrollElement

- parseSensorPropertyElement

- parseTemperatureElement

- parseUnicodeElement

- parseVendorMessageElement

- processDigitizerElements

- processGameControllerElements

- processLEDElements

- processMultiAxisElements

- processUnicodeElements

- serializeCharacterGestureState

- serializeDebugState

- setAccelProperties

- setAccelerationProperties

- setBiometricProperties

- setCompassProperties

- setDeviceOrientationProperties

- setDigitizerProperties

- setElementValue

- setGameControllerProperties

- setGyroProperties

- setKeyboardProperties

- setLEDProperties

- setMultiAxisProperties

- setProperties

- setRelativeProperties

- setScrollProperties

- setSensorProperties

- setSurfaceDimensions

- setTemperatureProperties

- setUnicodeProperties

- setVendorMessageProperties

### Type Methods

+ calibrateCenteredPreferredStateElement

+ calibrateJustifiedPreferredStateElement

## Relationships

### Inherits From

- IOHIDEventService

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

