

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserStartController 

Instance Method

# UserStartController

Starts the controller in response to a call from the framework.

DriverKit

``` source
kern_return_t UserStartController();
```

## Return Value

A value that indicates the result of initialization. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

The framework always calls UserStartController before sending any requests to the driver for execution. The framework calls this method after UserInitializeController to start the services that the specific host bus adapter (HBA) dext driver provides. After completing this call, all services provided by the HBA driver are available to the client.

The following sample implementation of UserStartController sets its local power state to kIOServicePowerCapabilityOn, then calls a hypothetical `EnableReplyInterrupt()` convenience function. Next, it enables the interrupt dispatch source, and returns kIOReturnSuccess. Signaling success like this indicates to the kernel that the dext is now up and ready to serve I/O.

```
kern_return_t
IMPL ( ExampleSCSIDext, UserStartController )
{

    kern_return_t ret = kIOReturnError;

    ivars->fCurrentPowerState = kIOServicePowerCapabilityOn;

    // Enable interrupts on the hardware
    EnableReplyInterrupt ( );

    // Enable interrupt event source
    ret = ivars->fIntSource->SetEnable ( true );
    __Require ( ( kIOReturnSuccess == ret ), Exit );

    …
}
```

## See Also

### Managing Controllers

UserInitializeController

Initializes the controller in response to a call from the framework.

