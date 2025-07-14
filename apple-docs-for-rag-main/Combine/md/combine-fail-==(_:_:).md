

- Combine
- Fail
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Fail, rhs: Fail) -> Bool
```

Available when `Failure` conforms to `Equatable` and `Error`.

## Parameters 

`lhs`  

A `Fail` publisher to compare for equality.

`rhs`  

Another `Fail` publisher to compare for equality.

## Return Value

`true` if the publishers have equal `error` properties; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

