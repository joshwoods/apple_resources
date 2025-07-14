

- HIDDriverKit
- IOHIDElementCommitDirection
-  kIOHIDElementCommitDirectionOut 

Enumeration Case

# kIOHIDElementCommitDirectionOut

Causes the element data to be sent to the device.

DriverKitmacOS

``` source
kIOHIDElementCommitDirectionOut
```

## Discussion

Specifying this direction causes the commit function to send the element data to the device. Use the setValue or setDataValue functions to specify the new data before committing it.

## See Also

### Getting the Commit Directions

kIOHIDElementCommitDirectionIn

Causes the retrieval of information from the device, and the populating of the element with the resulting data.

