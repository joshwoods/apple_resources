

- Combine
- Publishers
- Publishers.Drop
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Drop, rhs: Publishers.Drop) -> Bool
```

Available when `Upstream` conforms to `Publisher` and `Equatable`.

## Parameters 

`lhs`  

A drop publisher to compare for equality.

`rhs`  

Another drop publisher to compare for equality.

## Return Value

`true` if the publishers have equal `upstream` and `count` properties; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

