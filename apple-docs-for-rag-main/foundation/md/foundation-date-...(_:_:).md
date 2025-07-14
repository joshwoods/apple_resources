

- Foundation
- Date
-  ...(\_:\_:) 

Operator

# ...(\_:\_:)

Returns a closed range that contains both of its bounds.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func ... (minimum: Self, maximum: Self) -> ClosedRange
```

## Parameters 

`minimum`  

The lower bound for the range.

`maximum`  

The upper bound for the range.

## Discussion

Use the closed range operator (`...`) to create a closed range of any type that conforms to the `Comparable` protocol. This example creates a `ClosedRange` from “a” up to, and including, “z”.

```
let lowercase = "a"..."z"
print(lowercase.contains("z"))
// Prints "true"
```

Precondition

`minimum 

## See Also

### Creating Date Ranges

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

