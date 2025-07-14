

- Swift
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func != (lhs: (A, B, C, D), rhs: (A, B, C, D)) -> Bool where A : Equatable, B : Equatable, C : Equatable, D : Equatable
```

## Parameters 

`lhs`  

A tuple of `Equatable` elements.

`rhs`  

Another tuple of elements of the same type as `lhs`.

## Discussion

For two tuples to compare as equal, each corresponding pair of components must be equal. The following example compares tuples made up of 4 components:

```
let a = ("a", 1, 2, 3)
let b = ("a", 1, 2, 3)
print(a != b)
// Prints "false"

let c = ("a", 1, 2, 4)
print(a != c)
// Prints "true"
```

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

func != ((), ()) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B>((A, B), (A, B)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C>((A, B, C), (A, B, C)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E>((A, B, C, D, E), (A, B, C, D, E)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

func != &lt;A, B, C, D, E, F>((A, B, C, D, E, F), (A, B, C, D, E, F)) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

