

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Int128
-  SignedInteger Implementations 

API Collection

# SignedInteger Implementations

## Topics

### Initializers

init&lt;T>(T)

Creates a new instance from the given integer.

init?&lt;T>(exactly: T)

### Instance Methods

func dividingFullWidth((high: Self, low: Self.Magnitude)) -> (quotient: Self, remainder: Self)

### Type Properties

static var isSigned: Bool

A Boolean value indicating whether this type is a signed integer type.

static var max: Self

The maximum representable integer in this type.

static var min: Self

The minimum representable integer in this type.

