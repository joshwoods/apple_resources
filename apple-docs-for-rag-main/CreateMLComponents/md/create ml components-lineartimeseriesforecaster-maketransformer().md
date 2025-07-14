

- Create ML Components
- LinearTimeSeriesForecaster
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized model suitable for incremental fitting.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func makeTransformer() -> LinearTimeSeriesForecaster.Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

