

- Swift
- Swift Standard Library
- Collections
- Range
-  RangeExpression Implementations 

API Collection

# RangeExpression Implementations

## Topics

### Operators

static func ~= (Self, Self.Bound) -> Bool

Returns a Boolean value indicating whether a value is included in a range.

### Instance Methods

func relative&lt;C>(to: C) -> Range&lt;Bound>

Returns the range of indices described by this range expression within the given collection.

