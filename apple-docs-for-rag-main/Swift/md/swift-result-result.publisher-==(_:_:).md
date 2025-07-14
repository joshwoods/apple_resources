

- Swift
- Result
- Result.Publisher
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: Result.Publisher.Output, Failure>.Publisher, rhs: Result.Publisher.Output, Failure>.Publisher) -> Bool
```

Available when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

