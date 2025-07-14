

- Screen Saver
-  ScreenSaverDefaults 

Class

# ScreenSaverDefaults

A class that defines a set of methods for saving and restoring user defaults for screen savers.

macOS 10.0+

``` source
class ScreenSaverDefaults
```

## Overview

ScreenSaverDefaults gives you access to preference values you need to configure your screen saver. Because multiple apps can load a screen saver, you can’t use the standard UserDefaults object to store preferences. Instead, instantiate this class using the init(forModuleWithName:) method, which takes your screen saver’s bundle identifier as a parameter. The resulting object gives you a way to store your preference values and associate them only with your screen saver. Use the inherited UserDefaults methods to load, store, or modify values.

## Topics

### Creating the screen saver defaults

convenience init?(forModuleWithName: String)

Returns a screen saver defaults instance that reads and writes defaults for the specified module.

## Relationships

### Inherits From

- UserDefaults

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Interface

class ScreenSaverView

An abstract class that defines the interface for subclassers to interact with the screen saver infrastructure.

