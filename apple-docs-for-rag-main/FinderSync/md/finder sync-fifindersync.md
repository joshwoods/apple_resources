

- Finder Sync
-  FIFinderSync 

Class

# FIFinderSync

A type to subclass to add badges, custom shortcut menus, and toolbar buttons to the Finder.

macOS 10.10+

``` source
class FIFinderSync
```

## Overview

Subclass the FIFinderSync class when you want to customize the appearance of the Finder. Although the FIFinderSync class doesn’t provide any developer accessible API, it does adopt the FIFinderSyncProtocol protocol. This protocol declares methods you can implement to modify the appearance of the Finder. For more information on these methods, see FIFinderSyncProtocol. To learn more about creating a Finder Sync extension, see Finder Sync in App Extension Programming Guide.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- FIFinderSyncProtocol
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Related Documentation

protocol FIFinderSyncProtocol

The group of methods to implement for modifying the Finder user interface to express file synchronization status and control.

### Classes

class FIFinderSyncController

A controller that acts as a bridge between your Finder Sync extension and the Finder itself.

