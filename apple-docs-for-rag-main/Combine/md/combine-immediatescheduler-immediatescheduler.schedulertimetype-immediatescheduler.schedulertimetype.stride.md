

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
-  ImmediateScheduler.SchedulerTimeType.Stride 

Structure

# ImmediateScheduler.SchedulerTimeType.Stride

The increment by which the immediate scheduler counts time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Stride
```

## Topics

### Creating Scheduler Time Strides

init(Int)

Creates an immediate scheduler time interval from the given time interval.

init?&lt;T>(exactly: T)

Creates an immediate scheduler time interval from a binary integer type.

init(floatLiteral: Double)

Creates an immediate scheduler time interval from a floating-point seconds value.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(integerLiteral: Int)

Creates an immediate scheduler time interval from an integer seconds value.

### Creating Scheduler Time Strides from Seconds

static func microseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of microseconds into an instance of this scheduler time type.

static func milliseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of milliseconds into an instance of this scheduler time type.

static func nanoseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of nanoseconds into an instance of this scheduler time type.

static func seconds(Double) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of seconds, as a floating-point value, into an instance of this scheduler time type.

static func seconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of seconds into an instance of this scheduler time type.

### Using Predefined Scheduler Time Strides

static var zero: Self

The zero value.

### Declaring Timekeeping Types

typealias FloatLiteralType

The type used when evaluating floating-point literals.

typealias IntegerLiteralType

The type used when evaluating integer literals.

typealias Magnitude

The type used for expressing the stride’s magnitude.

### Expressing Scheduler Time Strides as Seconds

var magnitude: Int

The value of this time interval in seconds.

### Creating Ranges

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

### Performing Mathematical Operations

func negate()

Replaces this value with its additive inverse.

static func * (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Multiplies two values and produces their product.

static func *= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Multiplies two values and stores the result in the left-hand-side variable.

static func + (Self) -> Self

Returns the given number unchanged.

static func + (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Adds two values and produces their sum.

static func += (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Adds two values and stores the result in the left-hand-side variable.

static func - (Self) -> Self

Returns the additive inverse of the specified value.

static func - (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Subtracts one value from another and produces their difference.

static func -= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

### Comparing Scheduler Time Strides

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Encoding Scheduler Time Strides

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Operators

static func &lt; (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Default Implementations

AdditiveArithmetic Implementations

Comparable Implementations

Equatable Implementations

SignedNumeric Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- Comparable
- Decodable
- Encodable
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Numeric
- SchedulerTimeIntervalConvertible
- SignedNumeric

