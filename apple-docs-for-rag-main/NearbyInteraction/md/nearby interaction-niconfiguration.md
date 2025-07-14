

- Nearby Interaction
-  NIConfiguration 

Class

# NIConfiguration

An abstract base class for interaction configurations.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
class NIConfiguration
```

## Mentioned in 

Initiating and maintaining a session

## Overview

The NIConfiguration class serves as the common identity for configuration objects. Don’t instantiate this class directly. Instead, instantiate one if its concrete subclasses: NINearbyPeerConfiguration or NINearbyAccessoryConfiguration. Use your configuration object to specify the features you want to enable in a Nearby Interaction session, and pass the object to the session’s run(_:) method.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NINearbyAccessoryConfiguration
- NINearbyPeerConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

