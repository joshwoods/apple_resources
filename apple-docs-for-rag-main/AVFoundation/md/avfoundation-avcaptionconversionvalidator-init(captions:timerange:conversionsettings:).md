

- AVFoundation
- AVCaptionConversionValidator
-  init(captions:timeRange:conversionSettings:) 

Initializer

# init(captions:timeRange:conversionSettings:)

Creates an object that validates captions for a conversion operation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    captions: [AVCaption],
    timeRange: CMTimeRange,
    conversionSettings: [AVCaptionSettingsKey : Any]
)
```

## Parameters 

`captions`  

The array of captions that the system validates.

`timeRange`  

The time range of the media timeline where the captions exist.

`conversionSettings`  

A dictionary that describes the conversion operation.

