

- Combine
- Publishers
- Publishers.MergeMany
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.MergeMany, rhs: Publishers.MergeMany) -> Bool
```

Available when `Upstream` conforms to `Publisher` and `Equatable`.

## Parameters 

`lhs`  

A `MergeMany` publisher to compare for equality.

`rhs`  

Another `MergeMany` publisher to compare for equality.

## Return Value

`true` if the publishers have equal `publishers` properties; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

