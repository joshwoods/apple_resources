

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- PartialRangeFrom
-  RangeExpression Implementations 

API Collection

# RangeExpression Implementations

## Topics

### Operators

static func ~= (Self, Self.Bound) -> Bool

Returns a Boolean value indicating whether a value is included in a range.

### Instance Methods

func contains(Bound) -> Bool

Returns a Boolean value indicating whether the given element is contained within the range expression.

func relative&lt;C>(to: C) -> Range&lt;Bound>

Returns the range of indices described by this range expression within the given collection.

