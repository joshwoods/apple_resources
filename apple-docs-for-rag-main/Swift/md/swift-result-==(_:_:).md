

- Swift
- Result
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (a: Result, b: Result) -> Bool
```

Available when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing Results

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

