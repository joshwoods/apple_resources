

- ScreenCaptureKit
- SCContentSharingPicker
-  defaultConfiguration 

Instance Property

# defaultConfiguration

The default configuration to use for the content capture picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
var defaultConfiguration: SCContentSharingPickerConfiguration { get set }
```

## See Also

### Stream configuration

func setConfiguration(SCContentSharingPickerConfiguration?, for: SCStream)

Sets the configuration for the content capture picker for a capture stream, providing allowed selection modes and content excluded from selection.

var configuration: SCContentSharingPickerConfiguration?

Sets the configuration for the content capture picker for all streams, providing allowed selection modes and content excluded from selection.

var maximumStreamCount: Int?

The maximum number of streams the content capture picker allows.

