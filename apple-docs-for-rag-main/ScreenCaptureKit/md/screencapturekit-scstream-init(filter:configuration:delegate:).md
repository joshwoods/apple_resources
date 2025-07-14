

- ScreenCaptureKit
- SCStream
-  init(filter:configuration:delegate:) 

Initializer

# init(filter:configuration:delegate:)

Creates a stream with a content filter and configuration.

Mac Catalyst 18.2+macOS 12.3+

``` source
init(
    filter contentFilter: SCContentFilter,
    configuration streamConfig: SCStreamConfiguration,
    delegate: (any SCStreamDelegate)?
)
```

## Parameters 

`contentFilter`  

The content to capture.

`streamConfig`  

The configuration to apply to the stream.

`delegate`  

An optional object that responds to stream events.

