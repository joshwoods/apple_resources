

- Kernel
- Hardware Families
- FireWire
-  IOFWDelayCommand 

Class

# IOFWDelayCommand

Command to execute some code after a specified delay (in microseconds) All it does is timeout after the specified delay, hence calling the completion callback.

macOS 10.0+

``` source
class IOFWDelayCommand : IOFWBusCommand
```

## Topics

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- execute

- getMetaClass

- initWithDelay

- reinit

## Relationships

### Inherits From

- IOFWBusCommand

