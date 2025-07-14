

- ScreenCaptureKit
- SCContentSharingPickerConfiguration
-  allowsChangingSelectedContent 

Instance Property

# allowsChangingSelectedContent

A Boolean value that indicates if the present stream can change to a different source.

Mac Catalyst 18.2+macOS 14.0+

``` source
var allowsChangingSelectedContent: Bool
```

## Discussion

The default value is `true`.

## See Also

### Control streaming selections

var allowedPickerModes: SCContentSharingPickerMode

The content-selection modes supported by the picker.

var excludedBundleIDs: Array&lt;String>

A list of bundle IDs to exclude from the sharing picker.

var excludedWindowIDs: Array&lt;Int>

A list of window IDs to exclude from the sharing picker.

