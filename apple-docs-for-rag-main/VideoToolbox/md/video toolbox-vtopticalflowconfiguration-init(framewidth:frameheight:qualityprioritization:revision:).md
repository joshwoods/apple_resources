

- Video Toolbox
- VTOpticalFlowConfiguration
-  init(frameWidth:frameHeight:qualityPrioritization:revision:) 

Initializer

# init(frameWidth:frameHeight:qualityPrioritization:revision:)

macOS 15.4+

``` source
init?(
    frameWidth: Int,
    frameHeight: Int,
    qualityPrioritization: VTOpticalFlowConfiguration.QualityPrioritization,
    revision: VTOpticalFlowConfiguration.Revision
)
```

## Parameters 

`frameWidth`  

The width of source frame in pixels. The maximum value is 8192 pixels for macOS, and 4096 pixels for iOS.

`frameHeight`  

The height of source frame in pixels. The maximum value is 4320 pixels for macOS, and 2160 pixels for iOS.

`qualityPrioritization`  

Instance to control quality and performance levels. See VEFrameRateConversionConfigurationQualityPrioritization for more information.

`revision`  

The specific algorithm or configuration revision that is to be used to perform the request.

