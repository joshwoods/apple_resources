

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Int128
-  Numeric Implementations 

API Collection

# Numeric Implementations

## Topics

### Operators

static func * (Int128, Int128) -> Int128

Multiplies two values and produces their product.

static func *= (inout Int128, Int128)

Multiplies two values and stores the result in the left-hand-side variable.

### Initializers

init?&lt;T>(exactly: T)

Creates a new instance from the given integer, if it can be represented exactly.

### Instance Properties

var magnitude: Int128.Magnitude

The magnitude of this value.

### Type Aliases

typealias Magnitude

A type that can represent the absolute value of any possible value of the conforming type.

