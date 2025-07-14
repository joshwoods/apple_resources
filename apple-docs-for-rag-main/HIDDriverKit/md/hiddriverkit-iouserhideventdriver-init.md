

- HIDDriverKit
- IOUserHIDEventDriver
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

### Running the Driver

Start

Starts the current event driver and associates it with the specified provider object.

free

Performs any final cleanup for the service.

