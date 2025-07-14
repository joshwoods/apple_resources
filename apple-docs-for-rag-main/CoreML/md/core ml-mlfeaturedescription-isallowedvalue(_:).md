

- Core ML
- MLFeatureDescription
-  isAllowedValue(\_:) 

Instance Method

# isAllowedValue(\_:)

Checks whether the model will accept an input feature value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func isAllowedValue(_ value: MLFeatureValue) -> Bool
```

## Parameters 

`value`  

Given the `MLFeatureValue`, is it compatible with the `MLFeatureType` of this `MLFeatureDescription`.

## Return Value

`True` if the given `MLFeatureValue` is acceptable to the model’s input feature, `false` otherwise.

