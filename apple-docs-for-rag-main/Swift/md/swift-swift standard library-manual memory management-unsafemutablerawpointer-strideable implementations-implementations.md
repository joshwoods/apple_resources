

- Swift
- Swift Standard Library
- Manual Memory Management
- UnsafeMutableRawPointer
-  Strideable Implementations 

API Collection

# Strideable Implementations

## Topics

### Operators

static func + (Self, Self.Stride) -> Self

static func + (Self.Stride, Self) -> Self

static func += (inout Self, Self.Stride)

static func - (Self, Self) -> Self.Stride

static func - (Self, Self.Stride) -> Self

static func -= (inout Self, Self.Stride)

### Instance Methods

func advanced(by: Int) -> UnsafeMutableRawPointer

Returns a value that is offset the specified distance from this value.

### Type Aliases

typealias Stride

A type that represents the distance between two values.

