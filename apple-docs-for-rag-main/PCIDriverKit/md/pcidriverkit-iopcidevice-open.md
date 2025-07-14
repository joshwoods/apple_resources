

- PCIDriverKit
- IOPCIDevice
-  Open 

Instance Method

# Open

Opens a session to the PCI device.

DriverKitmacOS

``` source
kern_return_t Open(IOService * forClient, IOOptionBits options);
```

## Parameters 

`forClient`  

The service object that is opening the session. Typically, you specify your driver’s custom IOService object.

`options`  

Additional options for opening the session.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method gives the specified IOService object exclusive access to the PCI device. It also gives the service object access to the PCI device’s configuration and aperture space.

## See Also

### Running the Service

init

Initializes the device.

Close

Closes the session to the PCI device.

free

Performs any final cleanup for the object.

