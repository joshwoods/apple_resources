

- Create ML Components
- LinearTimeSeriesForecaster
- LinearTimeSeriesForecaster.Model
-  export(to:metadata:) 

Instance Method

# export(to:metadata:)

Exports this transformer as a CoreML model package with user-supplied metadata.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func export(
    to url: URL,
    metadata: ModelMetadata
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`url`  

The location to write the model into.

`metadata`  

Contextual user-provided information.

