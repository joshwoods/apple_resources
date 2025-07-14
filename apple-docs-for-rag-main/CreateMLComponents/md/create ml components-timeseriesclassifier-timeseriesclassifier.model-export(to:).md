

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  export(to:) 

Instance Method

# export(to:)

Exports this transformer as a CoreML model package.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func export(to url: URL) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`url`  

The location to write the model into.

