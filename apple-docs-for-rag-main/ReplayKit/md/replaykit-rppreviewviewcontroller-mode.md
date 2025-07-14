

- ReplayKit
- RPPreviewViewController
-  mode 

Instance Property

# mode

The type of screen that appears when the view is presented.

tvOS 10.0+

``` source
@MainActor
var mode: RPPreviewViewControllerMode { get set }
```

## See Also

### Displaying the Preview UI

enum RPPreviewViewControllerMode

The modes used to determine whether the preview view controller or the share screen appears when editing a replay.

var previewControllerDelegate: (any RPPreviewViewControllerDelegate)?

The preview view controller’s delegate.

protocol RPPreviewViewControllerDelegate

The protocol you implement to respond to changes to a screen-recording user interface.

