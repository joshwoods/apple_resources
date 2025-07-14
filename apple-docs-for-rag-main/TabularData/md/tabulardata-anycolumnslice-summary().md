

- TabularData
- AnyColumnSlice
-  summary() 

Instance Method

# summary()

Generates a categorical summary of the column slice’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> AnyCategoricalSummary
```

## Discussion

The method tries to cast the the untyped column slice to a typed column slice before summarizing. Generating a summary for a typed column is faster and more efficient than for an untyped column.

