

- Combine
- Publishers
-  Publishers.Concatenate 

Structure

# Publishers.Concatenate

A publisher that emits all of one publisher’s elements before those from another publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Concatenate where Prefix : Publisher, Suffix : Publisher, Prefix.Failure == Suffix.Failure, Prefix.Output == Suffix.Output
```

## Topics

### Creating a Concatenate Publisher

init(prefix: Prefix, suffix: Suffix)

Creates a publisher that emits all of one publisher’s elements before those from another publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let prefix: Prefix

The publisher to republish, in its entirety, before republishing elements from `suffix`.

let suffix: Suffix

The publisher to republish only after `prefix` finishes.

### Comparing Publishers

static func == (Publishers.Concatenate&lt;Prefix, Suffix>, Publishers.Concatenate&lt;Prefix, Suffix>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

## See Also

### Applying Sequence Operations to Elements

struct DropUntilOutput

A publisher that ignores elements from the upstream publisher until it receives an element from second publisher.

struct Drop

A publisher that omits a specified number of elements before republishing later elements.

struct DropWhile

A publisher that omits elements from an upstream publisher until a given closure returns false.

struct TryDropWhile

A publisher that omits elements from an upstream publisher until a given error-throwing closure returns false.

struct PrefixWhile

A publisher that republishes elements while a predicate closure indicates publishing should continue.

struct TryPrefixWhile

A publisher that republishes elements while an error-throwing predicate closure indicates publishing should continue.

struct PrefixUntilOutput

A publisher that republishes elements until another publisher emits an element.

