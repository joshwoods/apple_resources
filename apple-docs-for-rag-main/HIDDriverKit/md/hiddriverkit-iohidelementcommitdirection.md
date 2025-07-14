

- HIDDriverKit
-  IOHIDElementCommitDirection 

Enumeration

# IOHIDElementCommitDirection

The commit direction for an HID element.

DriverKitmacOS

``` source
typedef enum { ... } IOHIDElementCommitDirection;
```

## Overview

Passing a value of kIOHIDElementCommitDirectionOut issues a setReport call to the device. Before issuing this call, set your desired value on the element with the setValue or setDataValue functions.

## Topics

### Getting the Commit Directions

kIOHIDElementCommitDirectionIn

Causes the retrieval of information from the device, and the populating of the element with the resulting data.

kIOHIDElementCommitDirectionOut

Causes the element data to be sent to the device.

## See Also

### Committing Changes to Elements

commit

Commits the element value to and from the device.

