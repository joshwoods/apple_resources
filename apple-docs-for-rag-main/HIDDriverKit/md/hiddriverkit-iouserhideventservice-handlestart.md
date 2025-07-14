

- HIDDriverKit
- IOUserHIDEventService
-  handleStart 

Instance Method

# handleStart

Performs additional initialization during the startup of the event service.

DriverKit 19.0+macOS

``` source
bool handleStart(IOService * provider);
```

## Parameters 

`provider`  

The `IOService` provider for this object.

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## Discussion

The default implemention of this method does nothing.

## See Also

### Running the Service

init

Handles the basic initialization of the event service.

Start

Starts the current event service and associates it with the specified provider object.

Stop

Stops the event service associated with the specified provider.

free

Performs any final cleanup for the service.

