

- Local Authentication
-  LADomainStateCompanion 

Class

# LADomainStateCompanion

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
class LADomainStateCompanion
```

## Topics

### Instance Properties

var availableCompanionTypes: Set&lt;LACompanionType>

var stateHash: Data?

Contains combined state hash data for all available companion types. . Returns `nil` if no companion devices are paired.

### Instance Methods

func stateHash(for: LACompanionType) -> Data?

Returns state hash data for the given companion type.

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

