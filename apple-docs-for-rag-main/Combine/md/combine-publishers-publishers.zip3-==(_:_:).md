

- Combine
- Publishers
- Publishers.Zip3
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Zip3, rhs: Publishers.Zip3) -> Bool
```

Available when `A` conforms to `Publisher`, `A` conforms to `Equatable`, `B` conforms to `Publisher`, `B` conforms to `Equatable`, `C` conforms to `Publisher`, `C` conforms to `Equatable`, `A.Failure` is `B.Failure`, and `B.Failure` is `C.Failure`.

## Parameters 

`lhs`  

A zip publisher to compare for equality.

`rhs`  

Another zip publisher to compare for equality.

## Return Value

`true` if the corresponding upstream publishers of each zip publisher are equal; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

