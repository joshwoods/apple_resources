

- Create ML Components
- NumericImputer
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized impute transformer suitable for incremental fitting.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> NumericImputer.Transformer
```

Available when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## Discussion

Note

You can’t use incremental fitting with an impute transformer when using the `median` strategy.

