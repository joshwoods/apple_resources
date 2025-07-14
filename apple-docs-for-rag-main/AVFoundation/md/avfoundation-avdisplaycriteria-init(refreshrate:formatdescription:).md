

- AVFoundation
- AVDisplayCriteria
-  init(refreshRate:formatDescription:) 

Initializer

# init(refreshRate:formatDescription:)

Creates a display criteria object with the specified refresh rate and format description.

tvOS 17.0+visionOS 1.0+

``` source
init(
    refreshRate: Float,
    formatDescription: CMFormatDescription
)
```

## Parameters 

`refreshRate`  

The requested screen refresh rate.

`formatDescription`  

An object that describes the format of the video.

