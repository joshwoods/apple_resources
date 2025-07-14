

- USBDriverKit
- IOUSBHostDevice
-  CreateInterfaceIterator 

Instance Method

# CreateInterfaceIterator

Creates an iterator to get the list of interfaces from the device.

DriverKit 19.0+

``` source
kern_return_t CreateInterfaceIterator(uintptr_t * ref);
```

## Parameters 

`ref`  

A pointer to a variable. On return, this variable contains an opaque iterator reference.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to create an iterator for the IOUSBHostInterface children belonging to this device. Pass the value you receive in the `ref` parameter to the CopyInterface method when fetching the interfaces.

## See Also

### Iterating Over the Device Interfaces

CopyInterface

Gets the next host interface child associated with this device.

DestroyInterfaceIterator

Destroys an interface iterator that you created.

