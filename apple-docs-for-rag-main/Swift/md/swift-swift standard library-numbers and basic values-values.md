

- Swift
- Swift Standard Library
-  Numbers and Basic Values 

API Collection

# Numbers and Basic Values

Model data with numbers, Boolean values, and other fundamental types.

## Topics

### Logical Values

struct Bool

A value type whose instances are either `true` or `false`.

### Numeric Values

struct Int

A signed integer value type.

struct Double

A double-precision, floating-point value type.

struct Float

A single-precision, floating-point value type.

### Ranges

struct Range

A half-open interval from a lower bound up to, but not including, an upper bound.

struct ClosedRange

An interval from a lower bound up to, and including, an upper bound.

### Errors

protocol Error

A type representing an error value that can be thrown.

enum Result

A value that represents either a success or a failure, including an associated value in each case.

### Optionals

enum Optional

A type that represents either a wrapped value or the absence of a value.

### Advanced Numerics

Numeric Protocols

Write generic code that works with any numeric type.

Special-Use Numeric Types

Work with fixed-width numeric types of different sizes.

SIMD Vector Types

Work with fixed-width vectors of fixed-width numeric types of different sizes.

Global Numeric Functions

Use these functions with numeric values and other comparable types.

### Random Number Generators

struct SystemRandomNumberGenerator

The system’s default source of random data.

protocol RandomNumberGenerator

A type that provides uniformly distributed random data.

## See Also

### Values and Collections

Strings and Text

Work with text using Unicode-safe strings.

Collections

Store and organize data using arrays, dictionaries, sets, and other data structures.

Time

Measure how long an operation takes and determine schedules in the future.

