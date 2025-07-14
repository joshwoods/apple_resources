

- Core ML
- MLSequence
-  type 

Instance Property

# type

The underlying type of the sequence’s elements.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var type: MLFeatureType { get }
```

## Discussion

The sequence’s underlying element type can only be either MLFeatureType.string or MLFeatureType.int64. Use this value to determine whether to access stringValues or int64Values at runtime.

