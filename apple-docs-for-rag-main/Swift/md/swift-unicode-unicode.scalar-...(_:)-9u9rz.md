

- Swift
- Unicode
- Unicode.Scalar
-  ...(\_:) 

Operator

# ...(\_:)

Returns a partial range extending upward from a lower bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func ... (minimum: Self) -> PartialRangeFrom
```

## Parameters 

`minimum`  

The lower bound for the range.

## Discussion

Use the postfix range operator (postfix `...`) to create a partial range of any type that conforms to the `Comparable` protocol. This example creates a `PartialRangeFrom` instance that includes any value greater than or equal to `5.0`.

```
let atLeastFive = 5.0...

atLeastFive.contains(4.0)     // false
atLeastFive.contains(5.0)     // true
atLeastFive.contains(6.0)     // true
```

You can use this type of partial range of a collection’s indices to represent the range from the partial range’s lower bound up to the end of the collection.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[3...])
// Prints "[40, 50, 60, 70]"
```

Precondition

`minimum` must compare equal to itself (i.e. cannot be NaN).

## See Also

### Creating Ranges of Scalars

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

