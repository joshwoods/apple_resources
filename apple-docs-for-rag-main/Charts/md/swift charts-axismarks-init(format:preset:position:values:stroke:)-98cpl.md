

- Swift Charts
- AxisMarks
-  init(format:preset:position:values:stroke:) 

Initializer

# init(format:preset:position:values:stroke:)

Creates axis markers with the given properties, will override default markers. Default content will be used for the axis markers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    format: Format,
    preset: AxisMarkPreset = .automatic,
    position: AxisMarkPosition = .automatic,
    values: [Value],
    stroke: StrokeStyle? = nil
) where Content == Never, Value : Plottable, Value == Format.FormatInput, Format : FormatStyle, Format.FormatOutput == String
```

## Parameters 

`format`  

The format to use for the labels.

`preset`  

The preset of the axis markers.

`position`  

The position of the axis markers.

`values`  

The values of the axis markers.

`stroke`  

The stroke to use for grid lines and ticks.

