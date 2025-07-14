

- Virtualization
-  VZMemoryBalloonDeviceConfiguration 

Class

# VZMemoryBalloonDeviceConfiguration

The common configuration traits for memory balloon devices.

macOS 11.0+

``` source
class VZMemoryBalloonDeviceConfiguration
```

## Overview

Don’t instantiate this abstract class directly. Instead, instantiate one of its subclasses such as VZVirtioTraditionalMemoryBalloonDeviceConfiguration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioTraditionalMemoryBalloonDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuration

class VZVirtioTraditionalMemoryBalloonDeviceConfiguration

A configuration object that provides a way to reclaim memory from the guest system.

