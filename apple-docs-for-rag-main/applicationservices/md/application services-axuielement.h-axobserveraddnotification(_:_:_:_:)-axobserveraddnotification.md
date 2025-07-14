

- Application Services
- AXUIElement.h
-  AXObserverAddNotification(\_:\_:\_:\_:) 

Function

# AXObserverAddNotification(\_:\_:\_:\_:)

Registers the specified observer to receive notifications from the specified accessibility object.

macOS 10.2+

``` source
func AXObserverAddNotification(
    _ observer: AXObserver,
    _ element: AXUIElement,
    _ notification: CFString,
    _ refcon: UnsafeMutableRawPointer?
) -> AXError
```

## Parameters 

`observer`  

The observer object created from a call to AXObserverCreate(_:_:_:).

`element`  

The accessibility object for which to observe notifications.

`notification`  

The name of the notification to observe.

`refcon`  

Application-defined data passed to the callback when it is called.

## Return Value

If unsuccessful, `AXObserverAddNotification` may return one of the following error codes, among others:

`kAXErrorInvalidUIElementObserver`  
The observer is not a valid AXObserverRef type.

`kAXErrorIllegalArgument`  
One or more of the arguments is an illegal value or the length of the notification name is greater than 1024.

`kAXErrorNotificationUnsupported`  
The accessibility object does not support notifications (note that the system-wide accessibility object does not support notifications).

`kAXErrorNotificationAlreadyRegistered`  
The notification has already been registered.

`kAXErrorCannotComplete`  
The function cannot complete because messaging has failed in some way.

`kAXErrorFailure`  
There is some sort of system memory failure.

## See Also

### Notification API

func AXObserverCreate(pid_t, AXObserverCallback, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications from the specified application.

func AXObserverCreateWithInfoCallback(pid_t, AXObserverCallbackWithInfo, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications with an information dictionary from the specified application.

func AXObserverGetRunLoopSource(AXObserver) -> CFRunLoopSource

Returns the observer's run loop source.

func AXObserverGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXObserverRef type.

func AXObserverRemoveNotification(AXObserver, AXUIElement, CFString) -> AXError

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

