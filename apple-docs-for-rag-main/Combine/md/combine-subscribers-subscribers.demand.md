

- Combine
- Subscribers
-  Subscribers.Demand 

Structure

# Subscribers.Demand

A requested number of items, sent to a publisher from a subscriber through the subscription.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Demand
```

## Mentioned in 

Processing Published Elements with Subscribers

## Topics

### Creating a Demand

static func max(Int) -> Subscribers.Demand

Creates a demand for the given maximum number of elements.

### Using Special Demands

static let unlimited: Subscribers.Demand

A request for as many values as the publisher can produce.

static let none: Subscribers.Demand

A request for no elements from the publisher.

### Inspecing Demand Properties

var max: Int?

The number of requested values.

### Encoding and Decoding

func encode(to: any Encoder) throws

Encodes the demand to the provide encoder.

init(from: any Decoder) throws

Creates a demand instance from a decoder.

### Performing Mathematical Operations

static func * (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of multiplying a demand by an integer.

static func *= (inout Subscribers.Demand, Int)

Multiplies a demand by an integer, and assigns the result to the demand.

static func + (Subscribers.Demand, Subscribers.Demand) -> Subscribers.Demand

Returns the result of adding two demands. When adding any value to `.unlimited`, the result is `.unlimited`.

static func + (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of adding an integer to a demand.

static func += (inout Subscribers.Demand, Subscribers.Demand)

Adds two demands, and assigns the result to the first demand.

static func += (inout Subscribers.Demand, Int)

Adds an integer to a demand, and assigns the result to the demand.

static func - (Subscribers.Demand, Subscribers.Demand) -> Subscribers.Demand

Returns the result of subtracting one demand from another.

static func - (Subscribers.Demand, Int) -> Subscribers.Demand

Returns the result of subtracting an integer from a demand.

static func -= (inout Subscribers.Demand, Subscribers.Demand)

Subtracts one demand from another, and assigns the result to the first demand.

static func -= (inout Subscribers.Demand, Int)

Subtracts an integer from a demand, and assigns the result to the demand.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

### Comparing Demands

static func == (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func == (Subscribers.Demand, Int) -> Bool

Returns a Boolean value that indicates whether a demand requests the given number of elements.

static func == (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether a given number of elements matches the request of a given demand.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func != (Subscribers.Demand, Int) -> Bool

Returns a Boolean value that indicates whether a demand isn’t equal to an integer.

static func != (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether an integer is unequal to a demand.

### Operators

static func &lt; (Int, Subscribers.Demand) -> Bool

Returns a Boolean that indicates a given number of elements is less than the maximum specified by the demand.

static func > (Int, Subscribers.Demand) -> Bool

Returns a Boolean that indicates a given number of elements is greater than the maximum specified by the demand.

static func > (Subscribers.Demand, Int) -> Bool

Returns a Boolean that indicates whether the demand requests more than the given number of elements.

static func > (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean that indicates whether the first demand requests more elements than the second.

static func &lt; (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean that indicates whether the first demand requests fewer elements than the second.

static func &lt; (Subscribers.Demand, Int) -> Bool

Returns a Boolean that indicates whether the demand requests fewer than the given number of elements.

static func >= (Subscribers.Demand, Int) -> Bool

Returns a Boolean that indicates whether the first demand requests more or the same number of elements as the second.

static func &lt;= (Subscribers.Demand, Int) -> Bool

Returns a Boolean that indicates whether the demand requests fewer or the same number of elements as the given integer.

static func &lt;= (Int, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates a given number of elements is less than or equal the maximum specified by the demand.

static func >= (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean that indicates whether the first demand requests more or the same number of elements as the second.

static func >= (Int, Subscribers.Demand) -> Bool

Returns a Boolean that indicates a given number of elements is greater than or equal to the maximum specified by the demand.

static func &lt;= (Subscribers.Demand, Subscribers.Demand) -> Bool

Returns a Boolean value that indicates whether the first demand requests fewer or the same number of elements as the second.

### Instance Properties

var description: String

A textual representation of this instance.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

