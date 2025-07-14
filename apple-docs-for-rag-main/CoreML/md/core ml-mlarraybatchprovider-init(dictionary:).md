

- Core ML
- MLArrayBatchProvider
-  init(dictionary:) 

Initializer

# init(dictionary:)

Creates a batch provider based on feature names and their associated arrays of data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(dictionary: [String : [Any]]) throws
```

## Parameters 

`dictionary`  

A dictionary which maps feature names to an array of values. The error case occurs when all the arrays do not have the same length or the values in an aray are not expressible as an MLFeatureValue.

## Discussion

This initializer is convenient when the data are available as individual arrays.

```
let batch = try  MLArrayBatchProvider(dictionary: ["age": [30, 35, 29],
                                                   "weightLbs": [120.0, 170.4, 213.6]])
```

## See Also

### Initializers

init(array: [any MLFeatureProvider])

Creates the batch provider based on the array of feature providers.

