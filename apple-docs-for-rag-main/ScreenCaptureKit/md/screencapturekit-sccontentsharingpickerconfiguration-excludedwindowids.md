

- ScreenCaptureKit
- SCContentSharingPickerConfiguration
-  excludedWindowIDs 

Instance Property

# excludedWindowIDs

A list of window IDs to exclude from the sharing picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
var excludedWindowIDs: Array
```

## Discussion

Important

Using an invalid window ID can cause an error. Use window values returned from Core Graphics methods such as CGWindowListCopyWindowInfo(_:_:) to provide window IDs to exclude from the picker.

## See Also

### Control streaming selections

var allowedPickerModes: SCContentSharingPickerMode

The content-selection modes supported by the picker.

var allowsChangingSelectedContent: Bool

A Boolean value that indicates if the present stream can change to a different source.

var excludedBundleIDs: Array&lt;String>

A list of bundle IDs to exclude from the sharing picker.

