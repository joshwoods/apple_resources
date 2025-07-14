

- Combine
- Publishers
- Publishers.Sequence
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Sequence, rhs: Publishers.Sequence) -> Bool
```

Available when `Elements` conforms to `Equatable`, `Elements` conforms to `Sequence`, and `Failure` conforms to `Error`.

## Parameters 

`lhs`  

A `Sequence` publisher to compare for equality.

`rhs`  

Another `Sequewnce` publisher to compare for equality.

## Return Value

`true` if the publishers have equal `sequence` properties; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

