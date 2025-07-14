

- Swift
- Comparable
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

### Ranges

struct Range

A half-open interval from a lower bound up to, but not including, an upper bound.

struct RangeSet

A set of values of any comparable type, represented by ranges.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

struct ClosedRange

An interval from a lower bound up to, and including, an upper bound.

