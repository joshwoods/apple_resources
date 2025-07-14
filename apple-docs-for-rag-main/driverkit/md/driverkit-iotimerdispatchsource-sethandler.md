

- DriverKit
- IOTimerDispatchSource
-  SetHandler 

Instance Method

# SetHandler

Sets the handler block to run when the timer fires.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetHandler(OSAction * action);
```

## Parameters 

`action`  

The OSAction object that contains your custom callback method. The dispatch source object retains your action object until you call this method again or cancel the dispatch source.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Configuring the Timer Source

Create

Creates and configures a timer dispatch object.

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the timer dispatch source.

