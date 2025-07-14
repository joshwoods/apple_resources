

- HIDDriverKit
- IOHIDInterface
-  commitElements 

Instance Method

# commitElements

Gets or sets the contents of the interface’s stored elements.

DriverKit 19.0+macOS

``` source
kern_return_t commitElements(OSArray * elements, IOHIDElementCommitDirection direction);
```

## Parameters 

`elements`  

An array of IOHIDElement objects.

`direction`  

The direction in which to commit changes. Specify kIOHIDElementCommitDirectionIn to read the element data from the device. Specify kIOHIDElementCommitDirectionOut to write the element data to the device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Accessing the Elements of a Report

getElements

Returns the array of elements that the interface uses to store parsed report data.

