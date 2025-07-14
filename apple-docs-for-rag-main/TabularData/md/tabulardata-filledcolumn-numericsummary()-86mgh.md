

- TabularData
- FilledColumn
-  numericSummary() 

Instance Method

# numericSummary()

Generates a numeric summary of the floating-point column’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func numericSummary() -> NumericSummary
```

Available when `Base` conforms to `OptionalColumnProtocol` and `Base.WrappedElement` conforms to `BinaryFloatingPoint`.

## See Also

### Summarizing a Column

func summary() -> CategoricalSummary&lt;FilledColumn&lt;Base>.WrappedElement>

Generates a categorical summary of the filled column’s elements, including default values.

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column’s elements.

