

- Core ML
- MLFeatureProvider
-  featureValue(for:) 

Instance Method

# featureValue(for:)

Accesses the feature value given the feature’s name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func featureValue(for featureName: String) -> MLFeatureValue?
```

**Required**

## Parameters 

`featureName`  

The name of the feature of the desired value.

## Return Value

The value of the feature, or nil if no value exists for that name.

## See Also

### Accessing Values

var featureNames: Set&lt;String>

The set of valid feature names.

**Required**

