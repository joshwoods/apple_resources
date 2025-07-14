

- USBDriverKit
- IOUSBHostDevice
-  DestroyInterfaceIterator 

Instance Method

# DestroyInterfaceIterator

Destroys an interface iterator that you created.

DriverKit 19.0+

``` source
kern_return_t DestroyInterfaceIterator(uintptr_t ref);
```

## Parameters 

`ref`  

An opaque iterator reference that you created using the CreateInterfaceIterator method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Iterating Over the Device Interfaces

CreateInterfaceIterator

Creates an iterator to get the list of interfaces from the device.

CopyInterface

Gets the next host interface child associated with this device.

