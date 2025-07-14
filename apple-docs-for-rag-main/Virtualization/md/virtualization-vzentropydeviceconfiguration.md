

- Virtualization
-  VZEntropyDeviceConfiguration 

Class

# VZEntropyDeviceConfiguration

The common configuration traits for entropy devices.

macOS 11.0+

``` source
class VZEntropyDeviceConfiguration
```

## Overview

Don’t create a VZEntropyDeviceConfiguration object directly. Instead, instantiate a subclass such as VZVirtioEntropyDeviceConfiguration to configure a source of entropy for your virtual machine.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioEntropyDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZVirtioEntropyDeviceConfiguration

A source of entropy for the guest’s random number generator.

