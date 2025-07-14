

- Swift
- Optional
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether the left-hand-side argument is not `nil`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func != (lhs: borrowing Wrapped?, rhs: _OptionalNilComparisonType) -> Bool
```

## Parameters 

`lhs`  

A value to compare to `nil`.

`rhs`  

A `nil` literal.

## Discussion

You can use this not-equal-to operator (`!=`) to test whether an optional instance is not `nil` even when the wrapped value’s type does not conform to the `Equatable` protocol.

The following example declares the `stream` variable as an optional instance of a hypothetical `DataStream` type. Although `DataStream` is not an `Equatable` type, this operator allows checking whether `stream` wraps a value and is therefore not `nil`.

```
var stream: DataStream? = fetchDataStream()
if stream != nil {
    print("The data stream has been configured.")
}
// Prints "The data stream has been configured."
```

## See Also

### Comparing Optional Values

static func == (borrowing Wrapped?, _OptionalNilComparisonType) -> Bool

Returns a Boolean value indicating whether the left-hand-side argument is `nil`.

static func == (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether the right-hand-side argument is `nil`.

static func != (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether the right-hand-side argument is not `nil`.

static func ~= (_OptionalNilComparisonType, borrowing Wrapped?) -> Bool

Returns a Boolean value indicating whether an argument matches `nil`.

