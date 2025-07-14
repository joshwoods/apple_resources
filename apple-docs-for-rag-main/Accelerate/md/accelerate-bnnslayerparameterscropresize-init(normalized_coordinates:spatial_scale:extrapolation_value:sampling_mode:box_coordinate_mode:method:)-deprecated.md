

- Accelerate
- BNNSLayerParametersCropResize
-  init(normalized_coordinates:spatial_scale:extrapolation_value:sampling_mode:box_coordinate_mode:method:) Deprecated

Initializer

# init(normalized_coordinates:spatial_scale:extrapolation_value:sampling_mode:box_coordinate_mode:method:)

Creates a new layer parameters structure.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
init(
    normalized_coordinates: Bool,
    spatial_scale: Float,
    extrapolation_value: Float,
    sampling_mode: BNNSLinearSamplingMode,
    box_coordinate_mode: BNNSBoxCoordinateMode,
    method: BNNSInterpolationMethod
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`normalized_coordinates`  

A Boolean value that specifies whether the operation treats the coordinates as normalized to `0...1`.

`spatial_scale`  

An additional spatial scale that mutliplies the bounding box coordinates.

`extrapolation_value`  

A value that the operation uses for extrapolation. Default value is `0`.

`sampling_mode`  

The sampling mode that the operation uses to select sample points.

`box_coordinate_mode`  

A constant that defines the convention for the operation uses to specify the four bounding box coordinates.

`method`  

The interpolation method.

## See Also

### Initializers

init()

Creates a new empty layer parameters structure.

Deprecated

