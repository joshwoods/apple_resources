

- Spatial
-  Angle2D 

Structure

# Angle2D

A geometric angle with a value you access in either radians or degrees.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Angle2D
```

## Topics

### Creating an angle structure

init()

Creates an angle.

init(Angle)

Creates an angle from a SwiftUI angle.

init(radians: Double)

Creates an angle with the specified double-precision radians.

init(radians: Double)

Creates an angle with the specified double-precision radians.

init&lt;T>(radians: T)

Creates an angle with the specified floating-point radians.

init&lt;T>(degrees: T)

Creates an angle with the specified floating-point degrees.

init(degrees: Double)

Creates an angle with the specified double-precision degrees.

static func degrees(Double) -> Angle2D

Returns a new angle structure with the specified double-precision degrees.

static func radians(Double) -> Angle2D

Returns a new angle structure with the specified double-precision radians.

### Inspecting an angle’s properties

var degrees: Double

The angle in degrees.

var radians: Double

The angle in radians.

### Geometry functions

func cos(Angle2D) -> Double

Returns the cosine of the specified angle.

func cosh(Angle2D) -> Double

Returns the hyperbolic cosine of the specified angle.

func sin(Angle2D) -> Double

Returns the sine of the specified angle.

func sinh(Angle2D) -> Double

Returns the hyperbolic sine of the specified angle.

func tan(Angle2D) -> Double

Returns the tangent of the specified angle.

func tanh(Angle2D) -> Double

Returns the hyperbolic tangent of the specified angle.

static func acos(Double) -> Angle2D

Returns the inverse cosine of the specified value.

static func acosh(Double) -> Angle2D

Returns the inverse hyperbolic cosine of the specified value.

static func asin(Double) -> Angle2D

Returns the inverse sine of the specified value.

static func asinh(Double) -> Angle2D

Returns the inverse hyperbolic sine of the specified value.

static func atan(Double) -> Angle2D

Returns the inverse hyperbolic tangent of the specified value.

static func atan2(y: Double, x: Double) -> Angle2D

Returns the two-argument arctangent of the specified values.

static func atanh(Double) -> Angle2D

Returns the inverse hyperbolic tangent of the specified value.

var normalized: Angle2D

Returns the specified angle normalized between –180° and 180.0°.

### Comparing values

static func == (Angle2D, Angle2D) -> Bool

Returns a Boolean value that indicates whether two angles are equal.

### Encoding and decoding an angle structure

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Applying arithmetic operations

static func + (Angle2D) -> Angle2D

Returns the given angle unchanged.

static func + (Angle2D, Angle2D) -> Angle2D

Adds two angles and produces their sum.

static func += (inout Angle2D, Angle2D)

Adds two angles and stores the result in the left-hand-side variable.

static func - (Angle2D) -> Angle2D

Returns the additive inverse of the given angle.

static func - (Angle2D, Angle2D) -> Angle2D

Subtracts one angle from another and produces their difference.

static func -= (inout Angle2D, Angle2D)

Subtracts the second angle from the first and stores the difference in the left-hand-side variable.

### Default Implementations

AdditiveArithmetic Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- Animatable
- BitwiseCopyable
- Copyable
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

