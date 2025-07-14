

- PHASE
-  PHASEDirectivityModelParameters 

Class

# PHASEDirectivityModelParameters

A base class for objects that direct sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEDirectivityModelParameters
```

## Overview

Several classes derive from this class that implement a unique strategy to direct sound. Rather than create an instance of this class, instantiate a subclass, such as PHASECardioidDirectivityModelParameters or PHASEConeDirectivityModelParameters.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASECardioidDirectivityModelParameters
- PHASEConeDirectivityModelParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sound Directivity

class PHASECardioidDirectivityModelParameters

An object that directs sound in a heart-shaped curve surrounding a sound source.

class PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

class PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

class PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

