

- Combine
- Publishers
- Publishers.Merge5
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two publishers are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Publishers.Merge5, rhs: Publishers.Merge5) -> Bool
```

Available when `A` conforms to `Publisher`, `A` conforms to `Equatable`, `B` conforms to `Publisher`, `B` conforms to `Equatable`, `C` conforms to `Publisher`, `C` conforms to `Equatable`, `D` conforms to `Publisher`, `D` conforms to `Equatable`, `E` conforms to `Publisher`, `E` conforms to `Equatable`, `A.Failure` is `B.Failure`, `A.Output` is `B.Output`, `B.Failure` is `C.Failure`, `B.Output` is `C.Output`, `C.Failure` is `D.Failure`, `C.Output` is `D.Output`, `D.Failure` is `E.Failure`, and `D.Output` is `E.Output`.

## Parameters 

`lhs`  

A merging publisher to compare for equality.

`rhs`  

Another merging publisher to compare for equality.

## Return Value

`true` if the two merging publishers have equal source publishers; otherwise `false`.

## See Also

### Comparing Publishers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

