

- Matter
-  MTRAttributeValueWaiter 

Class

# MTRAttributeValueWaiter

iOS 18.3+iPadOS 18.3+Mac Catalyst 18.3+macOS 15.3+tvOS 18.3+visionOS 2.3+watchOS 11.3+

``` source
class MTRAttributeValueWaiter
```

## Topics

### Instance Properties

var uuid: UUID

### Instance Methods

func cancel()

Cancel the wait for the set of attribute path/value pairs represented by this MTRAttributeValueWaiter. If the completion has not been called yet, it will becalled with MTRErrorCodeCancelled.

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

