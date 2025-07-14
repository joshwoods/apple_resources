

- Swift
- PartialRangeThrough
-  ~=(\_:\_:) 

Operator

# ~=(\_:\_:)

Returns a Boolean value indicating whether a value is included in a range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func ~= (pattern: Self, value: Self.Bound) -> Bool
```

## Parameters 

`pattern`  

A range.

## Discussion

You can use the pattern-matching operator (`~=`) to test whether a value is included in a range. The pattern-matching operator is used internally in `case` statements for pattern matching. The following example uses the `~=` operator to test whether an integer is included in a range of single-digit numbers:

```
let chosenNumber = 3
if 0..

