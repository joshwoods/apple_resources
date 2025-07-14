

- HIDDriverKit
- IOHIDElementCommitDirection
-  kIOHIDElementCommitDirectionIn 

Enumeration Case

# kIOHIDElementCommitDirectionIn

Causes the retrieval of information from the device, and the populating of the element with the resulting data.

DriverKitmacOS

``` source
kIOHIDElementCommitDirectionIn
```

## Discussion

Specifying this direction causes the commit function to read the element data from the device and update the current object. You can access the resulting data using the getValue or getDataValue functions.

## See Also

### Getting the Commit Directions

kIOHIDElementCommitDirectionOut

Causes the element data to be sent to the device.

