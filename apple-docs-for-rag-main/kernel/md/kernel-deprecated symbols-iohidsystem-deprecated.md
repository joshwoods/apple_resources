

- Kernel
- Deprecated Symbols
-  IOHIDSystem Deprecated

Class

# IOHIDSystem

macOS 10.15.4–10.15.4Deprecated

``` source
class IOHIDSystem : IOService
```

## Topics

### Instance Methods

- animateWaitCursor

- attach

- changeCursor

- configureReport

- createFilteredParamPropertiesForService

- createParameters

- createShmem

- createShmemGated

- detach

- disableContinuousCursor

- dispatchEvent

- doProcessNotifications

- enableContinuousCursor

- evClose

- evCloseGated

- evDispatch

- evOpen

- evOpenGated

- eventFlags

- extGetButtonEventNum

- extGetButtonEventNumGated

- extGetStateForSelector

- extGetUserHidActivityState

- extPostEvent

- extPostEventGated

- extRegisterVirtualDisplay

- extSetBounds

- extSetMouseLocation

- extSetMouseLocationGated

- extSetOnScreenBounds

- extSetStateForSelector

- extSetVirtualDisplayBounds

- extUnregisterVirtualDisplay

- free

- genericNotificationHandler

- getMetaClass

- getUserHidActivityStateGated

- getWorkLoop

- hidActivityChecker

- hideCursor

- hideWaitCursor

- init

- initShmem

- keyboardEvent

- keyboardEvent

- keyboardEventGated

- keyboardSpecialEvent

- keyboardSpecialEvent

- keyboardSpecialEventGated

- message

- moveCursor

- newUserClient

- newUserClientGated

- periodicEvents

- pointToScreen

- postEvent

- probe

- registerEventQueue

- registerEventQueueGated

- registerEventSource

- registerScreen

- registerScreenGated

- reportUserHidActivityGated

- resetCursor

- scheduleNextPeriodicEvent

- setBounds

- setContinuousCursorEnable

- setContinuousCursorEnableGated

- setCursorEnable

- setCursorEnableGated

- setCursorPosition

- setDisplayBoundsGated

- setEventsEnable

- setParamProperties

- setParamPropertiesPostGated

- setParamPropertiesPreGated

- setProperties

- showCursor

- showWaitCursor

- sleepDisplayTickle

- start

- startCursor

- unregisterEventQueue

- unregisterEventQueueGated

- unregisterScreen

- unregisterScreenGated

- updateEventFlags

- updateEventFlags

- updateEventFlagsGated

- updateHidActivity

- updateParamPropertiesGated

- updatePowerState

- updateReport

- workspaceBounds

### Type Methods

+ doCreateShmem

+ doEvClose

+ doExtGetButtonEventNum

+ doExtGetStateForSelector

+ doExtPostEvent

+ doExtSetMouseLocation

+ doExtSetStateForSelector

+ doKeyboardEvent

+ doKeyboardSpecialEvent

+ doNewUserClient

+ doProcessKeyboardEQ

+ doRegisterEventQueue

+ doRegisterScreen

+ doSetContinuousCursorEnable

+ doSetCursorEnable

+ doSetDisplayBounds

+ doSetParamPropertiesPost

+ doSetParamPropertiesPre

+ doUnregisterEventQueue

+ doUnregisterScreen

+ doUpdateEventFlags

+ getUserHidActivityState

+ handlePublishNotification

+ handleTerminationNotification

+ instance

+ makeInt32ArrayParamProperty

+ makeNumberParamProperty

+ powerStateHandler

+ processKeyboardEQ

+ reportUserHidActivity

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

IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

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

