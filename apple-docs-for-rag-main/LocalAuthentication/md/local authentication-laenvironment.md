

- Local Authentication
-  LAEnvironment 

Class

# LAEnvironment

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
class LAEnvironment
```

## Topics

### Classes

class Mechanism

class MechanismBiometry

class MechanismCompanion

class MechanismUserPassword

class State

### Protocols

protocol Observer

### Instance Properties

var state: LAEnvironment.State

The environment state information.

### Instance Methods

func addObserver(any LAEnvironment.Observer)

func removeObserver(any LAEnvironment.Observer)

### Type Properties

class var currentUser: LAEnvironment

Environment of the current user.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

