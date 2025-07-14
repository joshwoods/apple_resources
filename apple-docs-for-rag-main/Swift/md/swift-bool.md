

- Swift
-  Bool 

Structure

# Bool

A value type whose instances are either `true` or `false`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Bool
```

## Overview

`Bool` represents Boolean values in Swift. Create instances of `Bool` by using one of the Boolean literals `true` or `false`, or by assigning the result of a Boolean method or operation to a variable or constant.

```
var godotHasArrived = false

let numbers = 1...5
let containsTen = numbers.contains(10)
print(containsTen)
// Prints "false"

let (a, b) = (100, 101)
let aFirst = a 

Swift uses only simple Boolean values in conditional contexts to help avoid accidental programming errors and to help maintain the clarity of each control statement. Unlike in other programming languages, in Swift, integers and strings cannot be used where a Boolean value is required.

For example, the following code sample does not compile, because it attempts to use the integer `i` in a logical context:

```
var i = 5
while i {
    print(i)
    i -= 1
}
// error: Cannot convert value of type 'Int' to expected condition type 'Bool'
```

The correct approach in Swift is to compare the `i` value with zero in the `while` statement.

```
while i != 0 {
    print(i)
    i -= 1
}
```

# Using Imported Boolean values

The C `bool` and `Boolean` types and the Objective-C `BOOL` type are all bridged into Swift as `Bool`. The single `Bool` type in Swift guarantees that functions, methods, and properties imported from C and Objective-C have a consistent type interface.

## Topics

### Comparing Boolean Values

static func == (Bool, Bool) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Transforming a Boolean

func toggle()

Toggles the Boolean variable’s value.

static func ! (Bool) -> Bool

Performs a logical NOT operation on a Boolean value.

static func || (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical OR operation on two Boolean values.

static func &amp;&amp; (Bool, @autoclosure () throws -> Bool) rethrows -> Bool

Performs a logical AND operation on two Boolean values.

### Creating a Random Value

static func random() -> Bool

Returns a random Boolean value.

static func random&lt;T>(using: inout T) -> Bool

Returns a random Boolean value, using the given generator as a source for randomness.

### Describing a Boolean

var description: String

A textual representation of the Boolean value.

### Inspecting a Boolean

var customMirror: Mirror

A mirror that reflects the `Bool` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Bool` instance.

Deprecated

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Creating a Boolean From Another Value

init(Bool)

Creates an instance equal to the given Boolean value.

init?(String)

Creates a new Boolean value from the given string.

### Converting an NSNumber to a Boolean

init(NSNumber)

init?(exactly: NSNumber)

init(truncating: NSNumber)

### Encoding and Decoding

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Using a Boolean as a Data Value

init?(from: MLDataValue)

Creates an instance of the conforming type from a data value.

var dataValue: MLDataValue

The value of the conforming type’s instance wrapped in a data value.

static var dataValueType: MLDataValue.ValueType

The underlying type the conforming type uses when it wraps itself in a data value.

### Infrequently Used Intializers

init()

Creates an instance initialized to `false`.

init(booleanLiteral: Bool)

Creates an instance initialized to the specified Boolean literal.

### Structures

struct IntentDisplayName

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

AtomicRepresentable Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByBooleanLiteral Implementations

Hashable Implementations

LosslessStringConvertible Implementations

MLDataValueConvertible Implementations

## Relationships

### Conforms To

- AtomicRepresentable
- BNNSScalar
- BindableData
- BitwiseCopyable
- CKRecordValueProtocol
- CVarArg
- Copyable
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByBooleanLiteral
- Hashable
- LosslessStringConvertible
- MLDataValueConvertible
- MLTensorScalar
- MusicLibraryRequestFilterValueEquatable
- Sendable

