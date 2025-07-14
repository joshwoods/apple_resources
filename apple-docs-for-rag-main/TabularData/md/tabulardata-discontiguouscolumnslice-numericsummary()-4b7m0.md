

- TabularData
- DiscontiguousColumnSlice
-  numericSummary() 

Instance Method

# numericSummary()

Generates a numeric summary of the floating-point column slice’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func numericSummary() -> NumericSummary
```

Available when `WrappedElement` conforms to `BinaryFloatingPoint`.

## See Also

### Summarizing a Column Slice

func summary() -> CategoricalSummary&lt;WrappedElement>

Generates a categorical summary of the column slice’s elements.

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column slice’s elements.

