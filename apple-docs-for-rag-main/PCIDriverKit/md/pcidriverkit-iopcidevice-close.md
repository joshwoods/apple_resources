

- PCIDriverKit
- IOPCIDevice
-  Close 

Instance Method

# Close

Closes the session to the PCI device.

DriverKitmacOS

``` source
void Close(IOService * forClient, IOOptionBits options);
```

## Parameters 

`forClient`  

The service object that is closing the session. If this object doesn’t have an open session to the device, this method does nothing..

`options`  

Additional options for closing the session.

## Discussion

This method closes the session previously opened by the object in the `forClient` parameter. The method also turns off the Bus Master Enable and Memory Space Enable bits defined in the command register of the PCI specification.

## See Also

### Running the Service

init

Initializes the device.

Open

Opens a session to the PCI device.

free

Performs any final cleanup for the object.

