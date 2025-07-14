

- HIDDriverKit
- IOUserHIDDevice
-  handleStart 

Instance Method

# handleStart

Performs any custom initialization associated with starting the device service.

DriverKit 19.0+macOS

``` source
bool handleStart(IOService * provider);
```

## Parameters 

`provider`  

The `IOService` provider for this object.

## Return Value

`true` if initialization was successful, or `false` if it wasn’t.

## Discussion

When defining a custom service, override this method and use it to perform any custom initialization. For example, you might allocate memory for your service’s instance variables and store a reference to the provider object for later use. The default implementation of this method returns `true`, and performs no other actions.

Don’t call this method yourself. The Start method calls it when starting up the service.

## See Also

### Running the Service

Start

Starts the device service and associates it with the specified provider object.

