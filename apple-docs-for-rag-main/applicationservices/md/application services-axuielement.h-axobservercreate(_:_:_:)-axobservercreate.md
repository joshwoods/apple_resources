

- Application Services
- AXUIElement.h
-  AXObserverCreate(\_:\_:\_:) 

Function

# AXObserverCreate(\_:\_:\_:)

Creates a new observer that can receive notifications from the specified application.

macOS 10.2+

``` source
func AXObserverCreate(
    _ application: pid_t,
    _ callback: AXObserverCallback,
    _ outObserver: UnsafeMutablePointer
) -> AXError
```

## Parameters 

`application`  

The process ID of the application.

`callback`  

The callback function.

`outObserver`  

On return, an AXObserverRef representing the observer object.

## Return Value

If unsuccessful, `AXObserverCreate` may return one of the following error codes, among others:

`kAXErrorIllegalArgument`  
One or more of the arguments is an illegal value.

`kAXErrorFailure`  
There is some sort of system memory failure.

## Discussion

When an observed notification is received, it is passed to AXObserverCallback.

## See Also

### Notification API

func AXObserverAddNotification(AXObserver, AXUIElement, CFString, UnsafeMutableRawPointer?) -> AXError

Registers the specified observer to receive notifications from the specified accessibility object.

func AXObserverCreateWithInfoCallback(pid_t, AXObserverCallbackWithInfo, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications with an information dictionary from the specified application.

func AXObserverGetRunLoopSource(AXObserver) -> CFRunLoopSource

Returns the observer's run loop source.

func AXObserverGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXObserverRef type.

func AXObserverRemoveNotification(AXObserver, AXUIElement, CFString) -> AXError

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

