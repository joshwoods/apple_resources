

- Virtualization
-  VZXHCIController 

Class

# VZXHCIController

A class that represents a USB Extensible Host Controller Interface (XHCI) controller in a VM.

macOS 15.0+

``` source
class VZXHCIController
```

## Overview

Don’t create `VZXHCIController` objects directly. Instead, you create a `VZXHCIController` object at runtime though the usbControllers property of the VZVirtualMachineConfiguration object by populating it with VZXHCIControllerConfiguration objects.

## Relationships

### Inherits From

- VZUSBController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Controllers

class VZUSBController

A class that represents a USB controller in a VM.

