

- Application Services
- AXUIElement.h
-  AXObserverCallback 

Type Alias

# AXObserverCallback

macOS 10.2+

``` source
typealias AXObserverCallback = (AXObserver, AXUIElement, CFString, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`observer`  

An AXObserverRef object to observe the notifications.

`element`  

The accessibility object.

`notification`  

The name of the notification to observe.

`refcon`  

Application-defined data specified when registering the observer for notification

## See Also

### Callbacks

typealias AXObserverCallbackWithInfo

