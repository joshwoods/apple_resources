

- Core ML
- MLArrayBatchProvider
-  init(array:) 

Initializer

# init(array:)

Creates the batch provider based on the array of feature providers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(array: [any MLFeatureProvider])
```

## Parameters 

`array`  

The array of feature providers for the batch.

## See Also

### Initializers

init(dictionary: [String : [Any]]) throws

Creates a batch provider based on feature names and their associated arrays of data.

