

- Swift
-  \

Operator

# \

Returns a Boolean value indicating whether the first tuple is ordered before the second in a lexicographical ordering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func  Bool
```

## Parameters 

`lhs`  

An empty tuple.

`rhs`  

An empty tuple.

## Discussion

An arity zero tuple is never strictly before another arity zero tuple in a lexicographical ordering.

## See Also

### Tuple Comparison

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

func > &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the first tuple is ordered after the second in a lexicographical ordering.

