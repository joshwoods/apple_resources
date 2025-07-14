

- Swift
- Set
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

## See Also

### Comparing Sets

static func == (Set&lt;Element>, Set&lt;Element>) -> Bool

Returns a Boolean value indicating whether two sets have equal elements.

func isSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a subset of the given set.

func isSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a subset of the given sequence.

func isStrictSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isStrictSubset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict subset of the given sequence.

func isSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a superset of the given set.

func isSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given sequence.

func isStrictSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isStrictSuperset&lt;S>(of: S) -> Bool

Returns a Boolean value that indicates whether the set is a strict superset of the given sequence.

func isDisjoint(with: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set has no members in common with the given set.

func isDisjoint&lt;S>(with: S) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given sequence.

