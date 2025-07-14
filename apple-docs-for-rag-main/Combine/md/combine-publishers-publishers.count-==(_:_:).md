

- Combine
- Publishers
- Publishers.Count
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent. /// - Parameters:

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Count, rhs: Publishers.Count) -> Bool
```

Available when `Upstream` conforms to `Publisher` and `Equatable`.

## Return Value

`true` if the two publishers’ `upstream` properties are equal; otherwise `false`.

## Discussion

- lhs: A `Count` instance to compare.

- rhs: Another `Count` instance to compare.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

