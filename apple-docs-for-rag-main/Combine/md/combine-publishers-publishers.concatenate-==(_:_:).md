

- Combine
- Publishers
- Publishers.Concatenate
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Concatenate, rhs: Publishers.Concatenate) -> Bool
```

Available when `Prefix` conforms to `Publisher`, `Prefix` conforms to `Equatable`, `Suffix` conforms to `Publisher`, `Suffix` conforms to `Equatable`, `Prefix.Failure` is `Suffix.Failure`, and `Prefix.Output` is `Suffix.Output`.

## Parameters 

`lhs`  

A concatenate publisher to compare for equality.

`rhs`  

Another concatenate publisher to compare for equality.

## Return Value

`true` if the two publishers’ `prefix` and `suffix` properties are equal; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

