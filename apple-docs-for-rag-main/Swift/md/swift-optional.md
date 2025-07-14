

- Swift
-  Optional 

Enumeration

# Optional

A type that represents either a wrapped value or the absence of a value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum Optional where Wrapped : ~Copyable
```

## Overview

You use the `Optional` type whenever you use optional values, even if you never type the word `Optional`. Swift’s type system usually shows the wrapped type’s name with a trailing question mark (`?`) instead of showing the full type name. For example, if a variable has the type `Int?`, that’s just another way of writing `Optional`. The shortened form is preferred for ease of reading and writing code.

The types of `shortForm` and `longForm` in the following code sample are the same:

```
let shortForm: Int? = Int("42")
let longForm: Optional = Int("42")
```

The `Optional` type is an enumeration with two cases. `Optional.none` is equivalent to the `nil` literal. `Optional.some(Wrapped)` stores a wrapped value. For example:

```
let number: Int? = Optional.some(42)
let noNumber: Int? = Optional.none
print(noNumber == nil)
// Prints "true"
```

You must unwrap the value of an `Optional` instance before you can use it in many contexts. Because Swift provides several ways to safely unwrap optional values, you can choose the one that helps you write clear, concise code.

The following examples use this dictionary of image names and file paths:

```
let imagePaths = ["star": "/glyphs/star.png",
                  "portrait": "/images/content/portrait.jpg",
                  "spacer": "/images/shared/spacer.gif"]
```

Getting a dictionary’s value using a key returns an optional value, so `imagePaths["star"]` has type `Optional` or, written in the preferred manner, `String?`.

## Optional Binding

To conditionally bind the wrapped value of an `Optional` instance to a new variable, use one of the optional binding control structures, including `if let`, `guard let`, and `switch`.

```
if let starPath = imagePaths["star"] {
    print("The star image is at '\(starPath)'")
} else {
    print("Couldn't find the star image")
}
// Prints "The star image is at '/glyphs/star.png'"
```

## Optional Chaining

To safely access the properties and methods of a wrapped instance, use the postfix optional chaining operator (postfix `?`). The following example uses optional chaining to access the `hasSuffix(_:)` method on a `String?` instance.

```
if imagePaths["star"]?.hasSuffix(".png") == true {
    print("The star image is in PNG format")
}
// Prints "The star image is in PNG format"
```

## Using the Nil-Coalescing Operator

Use the nil-coalescing operator (`??`) to supply a default value in case the `Optional` instance is `nil`. Here a default path is supplied for an image that is missing from `imagePaths`.

```
let defaultImagePath = "/images/default.png"
let heartPath = imagePaths["heart"] ?? defaultImagePath
print(heartPath)
// Prints "/images/default.png"
```

The `??` operator also works with another `Optional` instance on the right-hand side. As a result, you can chain multiple `??` operators together.

```
let shapePath = imagePaths["cir"] ?? imagePaths["squ"] ?? defaultImagePath
print(shapePath)
// Prints "/images/default.png"
```

## Unconditional Unwrapping

When you’re certain that an instance of `Optional` contains a value, you can unconditionally unwrap the value by using the forced unwrap operator (postfix `!`). For example, the result of the failable `Int` initializer is unconditionally unwrapped in the example below.

```
let number = Int("42")!
print(number)
// Prints "42"
```

You can also perform unconditional optional chaining by using the postfix `!` operator.

```
let isPNG = imagePaths["star"]!.hasSuffix(".png")
print(isPNG)
// Prints "true"
```

Unconditionally unwrapping a `nil` instance with `!` triggers a runtime error.

## Topics

### Creating an Optional Value

case some(Wrapped)

The presence of a value, stored as `Wrapped`.

init(consuming Wrapped)

Creates an instance that stores the given value.

### Creating a Nil Value

case none

The absence of a value.

init(nilLiteral: ())

Creates an instance initialized with `nil`.

### Transforming an Optional Value

func map&lt;E, U>((Wrapped) throws(E) -> U) throws(E) -> U?

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

func flatMap&lt;E, U>((Wrapped) throws(E) -> U?) throws(E) -> U?

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

### Coalescing Nil Values

func ?? &lt;T>(consuming T?, @autoclosure () throws -> T) rethrows -> T

Performs a nil-coalescing operation, returning the wrapped value of an `Optional` instance or a default value.

func ?? &lt;T>(consuming T?, @autoclosure () throws -> T?) rethrows -> T?

Performs a nil-coalescing operation, returning the wrapped value of an `Optional` instance or a default `Optional` value.

### Comparing Optional Values

static func == (borrowing Wrapped?, _OptionalNilComparisonType) -> Bool

Returns a Boolean value indicating whether the left-hand-side argument is `nil`.

static func == (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether the right-hand-side argument is `nil`.

static func != (borrowing Wrapped?, _OptionalNilComparisonType) -> Bool

Returns a Boolean value indicating whether the left-hand-side argument is not `nil`.

static func != (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether the right-hand-side argument is not `nil`.

static func ~= (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether an argument matches `nil`.

### Encoding and Decoding

func encode(to: any Encoder) throws

Encodes this optional value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Inspecting an Optional

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var unsafelyUnwrapped: Wrapped

The wrapped value of this instance, unwrapped without checking whether the instance is `nil`.

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var customMirror: Mirror

The custom mirror for this instance.

### Publishing an Optional

var publisher: Optional&lt;Wrapped>.Publisher

A Combine publisher that publishes this instance’s value to each subscriber exactly once, if it has any value at all.

struct Publisher

The type of a Combine publisher that publishes the value of a Swift optional instance to each subscriber exactly once, if the instance has any value at all.

### Deprecated

var hashValue: Int

The hash value.

### Instance Methods

func take() -> Optional&lt;Wrapped>

Takes the wrapped value being stored in this instance and returns it while also setting the instance to `nil`. If there is no value being stored in this instance, this returns `nil` instead.

### Type Aliases

typealias Body

typealias Specification

typealias TableRowBody

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: Wrapped.UnwrappedType.Specification

### Default Implementations

AtomicRepresentable Implementations

AttachmentContent Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomTestStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByNilLiteral Implementations

Hashable Implementations

RelationshipCollection Implementations

## Relationships

### Conforms To

- AtomicRepresentable

  Conforms when `Wrapped` conforms to `AtomicOptionalRepresentable`.

- AttachmentContent
- AxisContent
- AxisMark
- BitwiseCopyable

  Conforms when `Wrapped` conforms to `BitwiseCopyable` and `Escapable`.

- ChartContent
- Commands
- Copyable

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- CustomDebugStringConvertible

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- CustomReflectable

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- CustomTestStringConvertible
- CustomizableToolbarContent
- Decodable

  Conforms when `Wrapped` conforms to `Decodable`.

- DecodableWithConfiguration
- Encodable

  Conforms when `Wrapped` conforms to `Encodable`.

- EncodableWithConfiguration
- Equatable

  Conforms when `Wrapped` conforms to `Equatable`.

- ExpressibleByNilLiteral

  Conforms when `Wrapped` conforms to `Escapable`.

- Gesture
- Hashable

  Conforms when `Wrapped` conforms to `Hashable`.

- MapContent
- RelationshipCollection
- Sendable

  Conforms when `Wrapped` conforms to `Escapable` and `Sendable`.

- StoreContent
- TabContent
- TableColumnContent
- TableRowContent
- ToolbarContent
- View

