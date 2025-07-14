

- Matter
-  MTRServerAttribute 

Class

# MTRServerAttribute

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRServerAttribute
```

## Topics

### Initializers

init?(readonlyAttributeWithID: NSNumber, initialValue: [String : Any], requiredPrivilege: MTRAccessControlEntryPrivilege)

### Instance Properties

var attributeID: NSNumber

var isWritable: Bool

var requiredReadPrivilege: MTRAccessControlEntryPrivilege

var value: [String : Any]

### Instance Methods

func setValue([String : Any]) -> Bool

### Type Methods

class func newFeatureMapAttribute(withInitialValue: NSNumber) -> Self

Create an attribute description for a FeatureMap attribute with the provided value (expected to be an unsigned integer representing the value of the bitmap). This will automatically set requiredPrivilege to the right value for FeatureMap.

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
- Sendable

