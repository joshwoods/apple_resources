

- ClockKit
- CLKComplicationTemplateExtraLargeRingImage
-  init(imageProvider:fillFraction:ringStyle:) Deprecated

Initializer

# init(imageProvider:fillFraction:ringStyle:)

Creates a new template from the provided image, fill fraction, and ring style.

watchOS 7.0–9.0Deprecated

``` source
init(
    imageProvider: CLKImageProvider,
    fillFraction: Float,
    ringStyle: CLKComplicationRingStyle
)
```

## Parameters 

`imageProvider`  

The image provider for the main image. The system renders the image as a tinted template image, a bitmap image where only the opacity of the image matters. For more information, see Providing images for different appearances.

`fillFraction`  

A value between `0.0` and `1.0` that indicates how much of the ring fills.

`ringStyle`  

The ring’s style. For a complete list of styles, see CLKComplicationRingStyle.

