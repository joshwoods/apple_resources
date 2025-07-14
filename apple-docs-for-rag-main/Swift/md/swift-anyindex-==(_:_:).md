

- Swift
- AnyIndex
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two indices wrap equal underlying indices.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: AnyIndex, rhs: AnyIndex) -> Bool
```

## Parameters 

`lhs`  

An index to compare.

`rhs`  

Another index to compare.

## Discussion

The types of the two underlying indices must be identical.

