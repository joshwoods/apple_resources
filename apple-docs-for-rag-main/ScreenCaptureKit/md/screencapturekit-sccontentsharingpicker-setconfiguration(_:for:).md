

- ScreenCaptureKit
- SCContentSharingPicker
-  setConfiguration(\_:for:) 

Instance Method

# setConfiguration(\_:for:)

Sets the configuration for the content capture picker for a capture stream, providing allowed selection modes and content excluded from selection.

Mac Catalyst 18.2+macOS 14.0+

``` source
func setConfiguration(
    _ configuration: SCContentSharingPickerConfiguration?,
    for stream: SCStream
)
```

## Parameters 

`configuration`  

The configuration to set for the given capture stream. When this value is `nil`, changes the stream configuration to use defaultConfiguration.

`stream`  

The capture stream to set a configuration for. When this value is `nil`, applies to all currently active streams.

## See Also

### Stream configuration

var configuration: SCContentSharingPickerConfiguration?

Sets the configuration for the content capture picker for all streams, providing allowed selection modes and content excluded from selection.

var defaultConfiguration: SCContentSharingPickerConfiguration

The default configuration to use for the content capture picker.

var maximumStreamCount: Int?

The maximum number of streams the content capture picker allows.

