

- Core ML
- MLBatchProvider
-  features(at:) 

Instance Method

# features(at:)

Returns the feature provider at the given index.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func features(at index: Int) -> any MLFeatureProvider
```

**Required**

## Parameters 

`index`  

The index of the desired feature provider.

## Return Value

The feature provider at the given index.

## See Also

### Accessing Values

var count: Int

The number of feature providers in this batch.

**Required**

