

- Swift
-  \>=(\_:\_:) 

Operator

# \>=(\_:\_:)

Returns a Boolean value indicating whether the first tuple is ordered after or the same as the second in a lexicographical ordering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func >= (lhs: (A, B, C, D, E, F), rhs: (A, B, C, D, E, F)) -> Bool where A : Comparable, B : Comparable, C : Comparable, D : Comparable, E : Comparable, F : Comparable
```

## Parameters 

`lhs`  

A tuple of `Comparable` elements.

`rhs`  

Another tuple of elements of the same type as `lhs`.

## Discussion

Given two tuples `(a1, a2, ..., aN)` and `(b1, b2, ..., bN)`, the first tuple is after or the same as the second tuple if and only if `a1 > b1` or (`a1 == b1` and `(a2, ..., aN) >= (b2, ..., bN)`).

## See Also

### Tuple Comparison

func &lt; ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt; &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

func &lt;= ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func &lt;= &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered before or the same as the second in a lexicographical ordering.

func > ((), ()) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

func > &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

