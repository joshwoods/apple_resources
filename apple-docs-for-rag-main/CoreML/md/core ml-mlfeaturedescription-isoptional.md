

- Core ML
- MLFeatureDescription
-  isOptional 

Instance Property

# isOptional

A Boolean value that indicates whether this feature is optional.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var isOptional: Bool { get }
```

## Discussion

Optional values can be `nil`, for models that have inputs related to features being present or not.

## See Also

### Inspecting a Feature

var name: String

The name of this feature.

var type: MLFeatureType

The type of this feature.

enum MLFeatureType

The possible types for feature values, input features, and output features.

