

- Swift
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func != (lhs: (), rhs: ()) -> Bool
```

## Parameters 

`lhs`  

An empty tuple.

`rhs`  

An empty tuple.

## Discussion

All arity zero tuples are equal.

## See Also

### Tuple Comparison

func == ((), ()) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func == &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether the corresponding components of two tuples are equal.

func != &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D>((A, B, C, D), (A, B, C, D)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

