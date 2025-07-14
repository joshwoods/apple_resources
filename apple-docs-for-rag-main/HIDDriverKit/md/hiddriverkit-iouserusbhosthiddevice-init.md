

- HIDDriverKit
- IOUserUSBHostHIDDevice
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

Starts the current device service and associates it with the specified provider object.

handleStart

Performs any custom initialization associated with starting the device service.

Stop

Stops the device service associated with the specified provider.

free

Performs any final cleanup for the service.

