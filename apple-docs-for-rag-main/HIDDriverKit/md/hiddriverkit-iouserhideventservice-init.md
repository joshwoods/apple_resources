

- HIDDriverKit
- IOUserHIDEventService
-  init 

Instance Method

# init

Handles the basic initialization of the event service.

DriverKit 19.0+macOS

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## See Also

### Running the Service

Start

Starts the current event service and associates it with the specified provider object.

handleStart

Performs additional initialization during the startup of the event service.

Stop

Stops the event service associated with the specified provider.

free

Performs any final cleanup for the service.

