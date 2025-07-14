

- Application Services
- AXUIElement.h
-  AXObserverRemoveNotification(\_:\_:\_:) 

Function

# AXObserverRemoveNotification(\_:\_:\_:)

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

macOS 10.2+

``` source
func AXObserverRemoveNotification(
    _ observer: AXObserver,
    _ element: AXUIElement,
    _ notification: CFString
) -> AXError
```

## Parameters 

`observer`  

The observer object created from a call to AXObserverCreate(_:_:_:).

`element`  

The accessibility object for which this observer observes notifications.

`notification`  

The name of the notification to remove from the list of observed notifications.

## Return Value

If unsuccessful, `AXObserverRemoveNotification` may return one of the following error codes, among others:

`kAXErrorInvalidUIElementObserver`  
The observer is not a valid AXObserverRef type.

`kAXErrorIllegalArgument`  
One or more of the arguments is an illegal value or the length of the notification name is greater than 1024.

`kAXErrorNotificationUnsupported`  
The accessibility object does not support notifications (note that the system-wide accessibility object does not support notifications).

`kAXErrorNotificationNotRegistered`  
This observer has not registered for any notifications.

`kAXErrorCannotComplete`  
The function cannot complete because messaging has failed in some way.

`kAXErrorFailure`  
There is some sort of system memory failure.

## See Also

### Notification API

func AXObserverAddNotification(AXObserver, AXUIElement, CFString, UnsafeMutableRawPointer?) -> AXError

Registers the specified observer to receive notifications from the specified accessibility object.

func AXObserverCreate(pid_t, AXObserverCallback, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications from the specified application.

func AXObserverCreateWithInfoCallback(pid_t, AXObserverCallbackWithInfo, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications with an information dictionary from the specified application.

func AXObserverGetRunLoopSource(AXObserver) -> CFRunLoopSource

Returns the observer's run loop source.

func AXObserverGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXObserverRef type.

