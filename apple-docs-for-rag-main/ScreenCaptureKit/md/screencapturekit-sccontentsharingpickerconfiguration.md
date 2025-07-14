

- ScreenCaptureKit
-  SCContentSharingPickerConfiguration 

Structure

# SCContentSharingPickerConfiguration

An instance for configuring the system content-sharing picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
struct SCContentSharingPickerConfiguration
```

## Topics

### Initializers

init()

Initializes a picker configuration with default values.

### Control streaming selections

var allowedPickerModes: SCContentSharingPickerMode

The content-selection modes supported by the picker.

var allowsChangingSelectedContent: Bool

A Boolean value that indicates if the present stream can change to a different source.

var excludedBundleIDs: Array&lt;String>

A list of bundle IDs to exclude from the sharing picker.

var excludedWindowIDs: Array&lt;Int>

A list of window IDs to exclude from the sharing picker.

## See Also

### System content-sharing picker

class SCContentSharingPicker

An instance of a picker presented by the operating system for managing frame-capture streams.

struct SCContentSharingPickerMode

Available modes for selecting streaming content from a picker presented by the operating system.

protocol SCContentSharingPickerObserver

An observer protocol your app implements to receive messages from the operating system’s content picker.

