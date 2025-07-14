

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- SIMD Vector Types
- SIMD32
-  SIMD Implementations 

API Collection

# SIMD Implementations

## Topics

### Operators

static func &amp; (Self, Self) -> Self

static func &amp; (Self, Self.Scalar) -> Self

static func &amp; (Self.Scalar, Self) -> Self

static func &amp;* (Self, Self) -> Self

static func &amp;* (Self.Scalar, Self) -> Self

static func &amp;* (Self, Self.Scalar) -> Self

static func &amp;*= (inout Self, Self)

static func &amp;*= (inout Self, Self.Scalar)

static func &amp;+ (Self.Scalar, Self) -> Self

static func &amp;+ (Self, Self.Scalar) -> Self

static func &amp;+ (Self, Self) -> Self

static func &amp;+= (inout Self, Self)

static func &amp;+= (inout Self, Self.Scalar)

static func &amp;- (Self, Self.Scalar) -> Self

static func &amp;- (Self.Scalar, Self) -> Self

static func &amp;- (Self, Self) -> Self

static func &amp;-= (inout Self, Self.Scalar)

static func &amp;-= (inout Self, Self)

static func &amp;= (inout Self, Self.Scalar)

static func &amp;= (inout Self, Self)

static func &amp;&lt;&lt; (Self, Self.Scalar) -> Self

static func &amp;>> (Self.Scalar, Self) -> Self

static func &amp;>> (Self, Self.Scalar) -> Self

static func &amp;&lt;&lt; (Self.Scalar, Self) -> Self

static func &amp;>> (Self, Self) -> Self

static func &amp;&lt;&lt; (Self, Self) -> Self

static func &amp;>>= (inout Self, Self.Scalar)

static func &amp;>>= (inout Self, Self)

static func &amp;&lt;&lt;= (inout Self, Self)

static func &amp;&lt;&lt;= (inout Self, Self.Scalar)

static func * (Self.Scalar, Self) -> Self

static func * (Self, Self.Scalar) -> SelfDeprecated

static func * (Self, Self.Scalar) -> Self

static func * (Self.Scalar, Self) -> SelfDeprecated

static func * (Self, Self) -> SelfDeprecated

static func * (Self, Self) -> Self

static func *= (inout Self, Self)

static func *= (inout Self, Self)Deprecated

static func *= (inout Self, Self.Scalar)Deprecated

static func *= (inout Self, Self.Scalar)

static func + (Self.Scalar, Self) -> Self

static func + (Self, Self) -> SelfDeprecated

static func + (Self, Self.Scalar) -> Self

static func + (Self.Scalar, Self) -> SelfDeprecated

static func + (Self, Self.Scalar) -> SelfDeprecated

static func + (Self, Self) -> Self

static func += (inout Self, Self.Scalar)

static func += (inout Self, Self.Scalar)Deprecated

static func += (inout Self, Self)Deprecated

static func += (inout Self, Self)

static func - (Self) -> Self

static func - (Self, Self) -> Self

static func - (Self.Scalar, Self) -> Self

static func - (Self, Self.Scalar) -> SelfDeprecated

static func - (Self, Self) -> SelfDeprecated

static func - (Self, Self.Scalar) -> Self

static func - (Self.Scalar, Self) -> SelfDeprecated

static func -= (inout Self, Self)

static func -= (inout Self, Self)Deprecated

static func -= (inout Self, Self.Scalar)

static func -= (inout Self, Self.Scalar)Deprecated

static func .!= (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise inequality comparison.

static func .!= (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise inequality comparison.

static func .!= (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

A vector mask with the result of a pointwise inequality comparison.

static func .== (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

A vector mask with the result of a pointwise equality comparison.

static func .== (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise equality comparison.

static func .== (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise equality comparison.

static func .&lt; (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than comparison.

static func .> (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than comparison.

static func .> (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than comparison.

static func .&lt; (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than comparison.

static func .&lt; (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than comparison.

static func .> (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than comparison.

static func .>= (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than or equal comparison.

static func .>= (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than or equal comparison.

static func .&lt;= (Self, Self.Scalar) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than or equal comparison.

static func .&lt;= (Self, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than or equal comparison.

static func .>= (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise greater than or equal comparison.

static func .&lt;= (Self.Scalar, Self) -> SIMDMask&lt;Self.MaskStorage>

Returns a vector mask with the result of a pointwise less than or equal comparison.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two vectors are equal.

static func % (Self, Self) -> Self

static func | (Self, Self.Scalar) -> Self

static func ^ (Self, Self) -> Self

static func | (Self.Scalar, Self) -> Self

static func ^ (Self, Self.Scalar) -> Self

static func / (Self.Scalar, Self) -> Self

static func / (Self, Self) -> Self

static func / (Self, Self) -> Self

static func | (Self, Self) -> Self

static func / (Self, Self.Scalar) -> Self

static func ^ (Self.Scalar, Self) -> Self

static func % (Self, Self.Scalar) -> Self

static func % (Self.Scalar, Self) -> Self

static func / (Self.Scalar, Self) -> Self

static func / (Self, Self.Scalar) -> Self

static func |= (inout Self, Self.Scalar)

static func %= (inout Self, Self)

static func /= (inout Self, Self.Scalar)

static func |= (inout Self, Self)

static func /= (inout Self, Self)

static func /= (inout Self, Self)

static func ^= (inout Self, Self.Scalar)

static func ^= (inout Self, Self)

static func /= (inout Self, Self.Scalar)

static func %= (inout Self, Self.Scalar)

static func ~ (Self) -> Self

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

var leadingZeroBitCount: Self

var nonzeroBitCount: Self

var trailingZeroBitCount: Self

### Instance Methods

func addProduct(Self.Scalar, Self)

func addProduct(Self, Self)

func addProduct(Self, Self.Scalar)

func addingProduct(Self, Self.Scalar) -> Self

func addingProduct(Self, Self) -> Self

func addingProduct(Self.Scalar, Self) -> Self

func clamp(lowerBound: Self, upperBound: Self)

func clamp(lowerBound: Self, upperBound: Self)

func clamped(lowerBound: Self, upperBound: Self) -> Self

func clamped(lowerBound: Self, upperBound: Self) -> Self

func encode(to: any Encoder) throws

Encodes the scalars of this vector into the given encoder in an unkeyed container.

func formSquareRoot()

func hash(into: inout Hasher)

Hashes the elements of the vector using the given hasher.

func max() -> Self.Scalar

The greatest scalar in the vector.

func max() -> Self.Scalar

The greatest element in the vector.

func min() -> Self.Scalar

The least element in the vector.

func min() -> Self.Scalar

The least scalar in the vector.

func replace(with: Self, where: SIMDMask&lt;Self.MaskStorage>)

Replaces elements of this vector with elements of `other` in the lanes where `mask` is `true`.

func replace(with: Self.Scalar, where: SIMDMask&lt;Self.MaskStorage>)

Replaces elements of this vector with `other` in the lanes where `mask` is `true`.

func replacing(with: Self, where: SIMDMask&lt;Self.MaskStorage>) -> Self

Returns a copy of this vector, with elements replaced by elements of `other` in the lanes where `mask` is `true`.

func replacing(with: Self.Scalar, where: SIMDMask&lt;Self.MaskStorage>) -> Self

Returns a copy of this vector, with elements `other` in the lanes where `mask` is `true`.

func round(FloatingPointRoundingRule)

func rounded(FloatingPointRoundingRule) -> Self

A vector formed by rounding each lane of the source vector to an integral value according to the specified rounding `rule`.

func squareRoot() -> Self

func sum() -> Self.Scalar

The sum of the scalars in the vector.

func wrappedSum() -> Self.Scalar

Returns the sum of the scalars in the vector, computed with wrapping addition.

### Type Properties

static var one: Self

A vector with one in all lanes.

static var one: Self

A vector with one in all lanes.

static var zero: Self

A vector with zero in all lanes.

static var zero: Self

A vector with zero in all lanes.

### Type Methods

static func random(in: ClosedRange&lt;Self.Scalar>) -> Self

Returns a vector with random values from within the specified range in all lanes.

static func random(in: Range&lt;Self.Scalar>) -> Self

Returns a vector with random values from within the specified range in all lanes.

static func random&lt;T>(in: Range&lt;Self.Scalar>, using: inout T) -> Self

Returns a vector with random values from within the specified range in all lanes, using the given generator as a source for randomness.

static func random&lt;T>(in: ClosedRange&lt;Self.Scalar>, using: inout T) -> Self

Returns a vector with random values from within the specified range in all lanes, using the given generator as a source for randomness.

