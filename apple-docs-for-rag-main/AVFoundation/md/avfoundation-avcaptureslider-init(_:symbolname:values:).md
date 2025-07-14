

- AVFoundation
- AVCaptureSlider
-  init(\_:symbolName:values:) 

Initializer

# init(\_:symbolName:values:)

Creates a discrete slider control that selects a value from a list.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
@nonobjc
convenience init(
    _ localizedTitle: String,
    symbolName: String,
    values: [Float]
)
```

## Parameters 

`localizedTitle`  

A localized title that describes the slider’s action.

`symbolName`  

A symbol name from the SF Symbols library.

`values`  

An array of floating-point values.

## Discussion

Use discrete sliders when your app supports selecting from a specific list of values.

## See Also

### Creating a slider

convenience init(String, symbolName: String, in: ClosedRange&lt;Float>)

Creates a continuous slider control that selects a value from a bounded range.

convenience init(String, symbolName: String, in: ClosedRange&lt;Float>, step: Float)

Creates a discrete slider control that selects a stepped value from a bounded range.

