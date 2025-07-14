

- Local Authentication
-  LASecret 

Class

# LASecret

Data that’s protected by a persisted right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LASecret
```

## Overview

You create LASecret instances when you store an LAPersistedRight; you can’t create them directly.

## Topics

### Loading secret data

func loadData(completion: (Data?, (any Error)?) -> Void)

Retrieves data stored in a secret.

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

## See Also

### Persistence

class LARightStore

A container for data protected by a right.

class LAPersistedRight

A right that gates access to a key and a secret.

