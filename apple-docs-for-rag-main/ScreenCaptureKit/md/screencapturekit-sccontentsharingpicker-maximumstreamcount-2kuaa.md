

- ScreenCaptureKit
- SCContentSharingPicker
-  maximumStreamCount 

Instance Property

# maximumStreamCount

The maximum number of streams the content capture picker allows.

Mac Catalyst 18.2+macOS 14.0+

``` source
var maximumStreamCount: Int? { get set }
```

## Discussion

The default value is `1`.

## See Also

### Stream configuration

func setConfiguration(SCContentSharingPickerConfiguration?, for: SCStream)

Sets the configuration for the content capture picker for a capture stream, providing allowed selection modes and content excluded from selection.

var configuration: SCContentSharingPickerConfiguration?

Sets the configuration for the content capture picker for all streams, providing allowed selection modes and content excluded from selection.

var defaultConfiguration: SCContentSharingPickerConfiguration

The default configuration to use for the content capture picker.

