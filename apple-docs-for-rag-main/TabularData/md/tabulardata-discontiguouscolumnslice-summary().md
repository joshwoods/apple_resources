

- TabularData
- DiscontiguousColumnSlice
-  summary() 

Instance Method

# summary()

Generates a categorical summary of the column slice’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> CategoricalSummary
```

Available when `WrappedElement` conforms to `Hashable`.

## See Also

### Summarizing a Column Slice

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column slice’s elements.

func numericSummary() -> NumericSummary&lt;WrappedElement>

Generates a numeric summary of the floating-point column slice’s elements.

