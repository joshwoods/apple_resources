

- Application Services
- AXUIElement.h
-  AXObserverGetRunLoopSource(\_:) 

Function

# AXObserverGetRunLoopSource(\_:)

Returns the observer's run loop source.

macOS 10.2+

``` source
func AXObserverGetRunLoopSource(_ observer: AXObserver) -> CFRunLoopSource
```

## Parameters 

`observer`  

The observer object (created from a call to AXObserverCreate(_:_:_:)) for which to get the run loop source.

## Return Value

Returns the CFRunLoopSourceRef of the observer; NIL if you pass NIL in `observer`.

## Discussion

The observer must be added to a run loop before it can receive notifications. Note that releasing the AXObserverRef automatically removes the run loop source from the run loop (you can also do this explicitly by calling CFRunLoopRemoveSource(_:_:_:)).

`AXObserverGetRunLoopSource` might be used in code in this way:

 CFRunLoopAddSource(CFRunLoopGetCurrent(), AXObserverGetRunLoopSource(observer), kCFRunLoopDefaultMode);

## See Also

### Notification API

func AXObserverAddNotification(AXObserver, AXUIElement, CFString, UnsafeMutableRawPointer?) -> AXError

Registers the specified observer to receive notifications from the specified accessibility object.

func AXObserverCreate(pid_t, AXObserverCallback, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications from the specified application.

func AXObserverCreateWithInfoCallback(pid_t, AXObserverCallbackWithInfo, UnsafeMutablePointer&lt;AXObserver?>) -> AXError

Creates a new observer that can receive notifications with an information dictionary from the specified application.

func AXObserverGetTypeID() -> CFTypeID

Returns the unique type identifier for the AXObserverRef type.

func AXObserverRemoveNotification(AXObserver, AXUIElement, CFString) -> AXError

Removes the specified notification from the list of notifications the observer wants to receive from the accessibility object.

