

- Swift Charts
- AxisMarks
-  init(preset:position:values:content:) 

Initializer

# init(preset:position:values:content:)

Creates axis markers with the given properties, will override default markers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    preset: AxisMarkPreset = .automatic,
    position: AxisMarkPosition = .automatic,
    values: [Value],
    @AxisMarkBuilder content: @escaping () -> Content
) where Value : Plottable
```

## Parameters 

`preset`  

The preset of the axis markers.

`position`  

The position of the axis markers.

`values`  

The values of the axis markers.

`content`  

A result builder that returns the content of the axis marker.

