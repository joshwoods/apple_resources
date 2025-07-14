

- Combine
- Publishers
- Publishers.IgnoreOutput
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.IgnoreOutput, rhs: Publishers.IgnoreOutput) -> Bool
```

Available when `Upstream` conforms to `Publisher` and `Equatable`.

## Parameters 

`lhs`  

An ignore output publisher to compare for equality.

`rhs`  

Another ignore output publisher to compare for equality.

## Return Value

`true` if the two publishers have equal upstream publishers; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

