

- Application Services
- AXUIElement.h
-  AXObserverGetTypeID() 

Function

# AXObserverGetTypeID()

Returns the unique type identifier for the AXObserverRef type.

macOS 10.2+

``` source
func AXObserverGetTypeID() -> CFTypeID
```

## Return Value

Returns the CFTypeID of the AXObserverRef type.

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

func AXObserverRemoveNotification(AXObserver, AXUIElement, CFString) -> AXError

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

