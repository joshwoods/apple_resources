

- Swift
- Unicode
- Unicode.Scalar
-  ..\

Operator

# ..\

Returns a half-open range that contains its lower bound but not its upper bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func .. Range
```

## Parameters 

`minimum`  

The lower bound for the range.

`maximum`  

The upper bound for the range.

## Discussion

Use the half-open range operator (`..` from zero up to, but not including, 5.0.

```
let lessThanFive = 0.0..

Precondition

`minimum 

## See Also

### Creating Ranges of Scalars

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

