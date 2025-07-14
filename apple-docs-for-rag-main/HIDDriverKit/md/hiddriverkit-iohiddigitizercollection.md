

- HIDDriverKit
-  IOHIDDigitizerCollection 

Class

# IOHIDDigitizerCollection

A collection of elements that contain digitizer-related data.

DriverKitmacOS

``` source
class IOHIDDigitizerCollection;
```

## Topics

### Creating a Digitizer Collection

withType

initWithType

free

IOHIDDigitizerCollectionType

### Accessing the Coordinates

getX

getY

getZ

setX

setY

setZ

### Managing the Collection Elements

getParentCollection

addElement

getElements

### Accessing Touch Data

getTouch

setTouch

### Getting the Collection Attributes

getType

getInRange

setInRange

## Relationships

### Inherits From

- OSContainer

## See Also

### HID Device Data

IOHIDElement

An object that contains parsed information from a HID input report.

com.apple.developer.hid.virtual.device

A Boolean value that indicates whether the driver creates a virtual HID device.

Low-Level Information

Understand the underlying structures that support HID drivers.

