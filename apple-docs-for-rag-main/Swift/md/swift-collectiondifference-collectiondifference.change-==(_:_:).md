

- Swift
- CollectionDifference
- CollectionDifference.Change
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (a: CollectionDifference.Change, b: CollectionDifference.Change) -> Bool
```

Available when `ChangeElement` conforms to `Equatable`.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

