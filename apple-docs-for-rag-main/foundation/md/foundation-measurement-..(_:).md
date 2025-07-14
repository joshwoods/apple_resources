

- Foundation
- Measurement
-  ..\

Operator

# ..\

Returns a partial range up to, but not including, its upper bound.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func .. PartialRangeUpTo
```

## Parameters 

`maximum`  

The upper bound for the range.

## Discussion

Use the prefix half-open range operator (prefix `..` instance that includes any value less than `5.0`.

```
let upToFive = ..

You can use this type of partial range of a collection’s indices to represent the range from the start of the collection up to, but not including, the partial range’s upper bound.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[..

Precondition

`maximum` must compare equal to itself (i.e. cannot be NaN).

## See Also

### Creating Ranges of Measurements

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

