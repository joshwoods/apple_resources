

- USBDriverKit
- IOUSBHostDevice
-  CopyInterface 

Instance Method

# CopyInterface

Gets the next host interface child associated with this device.

DriverKit 19.0+

``` source
kern_return_t CopyInterface(uintptr_t ref, IOUSBHostInterface * * interface);
```

## Parameters 

`ref`  

The opaque iterator reference you received from the CreateInterfaceIterator method.

`interface`  

A pointer to a variable. On output, this variable contains a pointer to the next IOUSBHostInterface object. When there are no more iterfaces, this method assigns `NULL` to the variable.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Keep calling this method until the value in the interface parameter is `NULL`.

## See Also

### Iterating Over the Device Interfaces

CreateInterfaceIterator

Creates an iterator to get the list of interfaces from the device.

DestroyInterfaceIterator

Destroys an interface iterator that you created.

