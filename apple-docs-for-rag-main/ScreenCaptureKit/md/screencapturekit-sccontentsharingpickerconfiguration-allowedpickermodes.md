

- ScreenCaptureKit
- SCContentSharingPickerConfiguration
-  allowedPickerModes 

Instance Property

# allowedPickerModes

The content-selection modes supported by the picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
var allowedPickerModes: SCContentSharingPickerMode
```

## Discussion

The default value doesn’t exclude selecting any content for streaming. There isn’t an equivalent SCContentSharingPickerMode available to reset this property once changed.

## See Also

### Control streaming selections

var allowsChangingSelectedContent: Bool

A Boolean value that indicates if the present stream can change to a different source.

var excludedBundleIDs: Array&lt;String>

A list of bundle IDs to exclude from the sharing picker.

var excludedWindowIDs: Array&lt;Int>

A list of window IDs to exclude from the sharing picker.

