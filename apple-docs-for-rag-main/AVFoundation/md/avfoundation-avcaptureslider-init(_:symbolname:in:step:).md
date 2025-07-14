

- AVFoundation
- AVCaptureSlider
-  init(\_:symbolName:in:step:) 

Initializer

# init(\_:symbolName:in:step:)

Creates a discrete slider control that selects a stepped value from a bounded range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
@nonobjc
convenience init(
    _ localizedTitle: String,
    symbolName: String,
    in range: ClosedRange,
    step: Float
)
```

## Parameters 

`localizedTitle`  

A localized title that describes the slider’s action.

`symbolName`  

A symbol name from the SF Symbols library.

`range`  

A bounded range of floating point values.

`step`  

The distance between each valid value. This specified value must be greater than `0` or the system throws an invalidArgumentException.

## Discussion

Use discrete sliders when your use case supports selecting stepped values within the specified range.

## See Also

### Creating a slider

convenience init(String, symbolName: String, in: ClosedRange&lt;Float>)

Creates a continuous slider control that selects a value from a bounded range.

convenience init(String, symbolName: String, values: [Float])

Creates a discrete slider control that selects a value from a list.

