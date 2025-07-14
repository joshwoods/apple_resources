

- Swift
- ContiguousArray
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two arrays contain the same elements in the same order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: ContiguousArray, rhs: ContiguousArray) -> Bool
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`lhs`  

An array to compare.

`rhs`  

Another array to compare.

## Discussion

You can use the equal-to operator (`==`) to compare any two arrays that store the same, `Equatable`-conforming element type.

