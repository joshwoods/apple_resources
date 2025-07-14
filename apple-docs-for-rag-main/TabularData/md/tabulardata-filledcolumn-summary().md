

- TabularData
- FilledColumn
-  summary() 

Instance Method

# summary()

Generates a categorical summary of the filled column’s elements, including default values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> CategoricalSummary.WrappedElement>
```

Available when `Base` conforms to `OptionalColumnProtocol` and `Base.WrappedElement` conforms to `Hashable`.

## See Also

### Summarizing a Column

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column’s elements.

func numericSummary() -> NumericSummary&lt;Base.WrappedElement>

Generates a numeric summary of the floating-point column’s elements.

