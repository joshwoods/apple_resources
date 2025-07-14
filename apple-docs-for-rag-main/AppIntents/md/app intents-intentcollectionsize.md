

- App Intents
-  IntentCollectionSize 

Structure

# IntentCollectionSize

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct IntentCollectionSize
```

## Topics

### Operators

static func == (IntentCollectionSize, IntentCollectionSize) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(exactly: Int)

init(integerLiteral: Int)

Creates an instance initialized to the specified integer value.

init(min: Int, max: Int)

### Type Aliases

typealias IntegerLiteralType

A type that represents an integer literal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByIntegerLiteral

## See Also

### Items and collections

struct IntentItem

A type describing a value returned from a dynamic options provider, plus information about how to display it to users.

struct IntentItemCollection

Return this object to provide an advanced list of options, optionally divided in sections.

struct IntentItemSection

An object you use to divide dynamic options into sections.

