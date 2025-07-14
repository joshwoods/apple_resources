

- HIDDriverKit
- IOHIDElement
-  commit 

Instance Method

# commit

Commits the element value to and from the device.

DriverKit 19.0+macOS

``` source
IOReturn commit(IOHIDElementCommitDirection direction);
```

## Parameters 

`direction`  

The direction to commit the element. Specify kIOHIDElementCommitDirectionIn to read the element data from the device. Specify kIOHIDElementCommitDirectionOut to write the element data to the device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Committing Changes to Elements

IOHIDElementCommitDirection

The commit direction for an HID element.

