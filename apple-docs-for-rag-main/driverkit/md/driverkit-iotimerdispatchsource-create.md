

- DriverKit
- IOTimerDispatchSource
-  Create 

Static Method

# Create

Creates and configures a timer dispatch object.

DriverKitiOSiPadOSmacOS

``` source
static kern_return_t Create(IODispatchQueue * queue, IOTimerDispatchSource * * source);
```

## Parameters 

`queue`  

The dispatch queue on which to run any handler blocks.

`source`  

A variable for storing the dispatch source. On return, this variable contains the retained object. You are responsible for releasing this object.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Configuring the Timer Source

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the timer dispatch source.

SetHandler

Sets the handler block to run when the timer fires.

