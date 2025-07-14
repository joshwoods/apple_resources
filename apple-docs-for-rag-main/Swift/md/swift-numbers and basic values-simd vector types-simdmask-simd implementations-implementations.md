

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- SIMD Vector Types
- SIMDMask
-  SIMD Implementations 

API Collection

# SIMD Implementations

## Topics

### Operators

static func .!= (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise inequality comparison.

static func .!= (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

A vector mask with the result of a pointwise inequality comparison.

static func .!= (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise inequality comparison.

static func .== (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise equality comparison.

static func .== (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise equality comparison.

static func .== (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

A vector mask with the result of a pointwise equality comparison.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two vectors are equal.

### Initializers

init&lt;S>(S)

Creates a vector from the given sequence.

init(arrayLiteral: Self.Scalar...)

Creates a vector from the specified elements.

init(from: any Decoder) throws

Creates a new vector by decoding scalars from the given decoder.

init(repeating: Self.Scalar)

A vector with the specified value in all lanes.

### Instance Properties

var description: String

A textual description of the vector.

var indices: Range&lt;Int>

The valid indices for subscripting the vector.

### Instance Methods

func encode(to: any Encoder) throws

Encodes the scalars of this vector into the given encoder in an unkeyed container.

func hash(into: inout Hasher)

Hashes the elements of the vector using the given hasher.

func replace(with: Self.Scalar, where: SIMDMask&lt;Self.MaskStorage>)

Replaces elements of this vector with `other` in the lanes where `mask` is `true`.

func replace(with: Self, where: SIMDMask&lt;Self.MaskStorage>)

Replaces elements of this vector with elements of `other` in the lanes where `mask` is `true`.

func replacing(with: Self, where: SIMDMask&lt;Self.MaskStorage>) -> Self

Returns a copy of this vector, with elements replaced by elements of `other` in the lanes where `mask` is `true`.

func replacing(with: Self.Scalar, where: SIMDMask&lt;Self.MaskStorage>) -> Self

Returns a copy of this vector, with elements `other` in the lanes where `mask` is `true`.

