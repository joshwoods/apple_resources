

- ReplayKit
-  RPPreviewViewControllerMode 

Enumeration

# RPPreviewViewControllerMode

The modes used to determine whether the preview view controller or the share screen appears when editing a replay.

tvOS 10.0+

``` source
enum RPPreviewViewControllerMode
```

## Topics

### Constants

case preview

Preview screen displayed when editing a replay.

case share

Share/AirDrop screen displayed when editing a replay.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Displaying the Preview UI

var mode: RPPreviewViewControllerMode

The type of screen that appears when the view is presented.

var previewControllerDelegate: (any RPPreviewViewControllerDelegate)?

The preview view controller’s delegate.

protocol RPPreviewViewControllerDelegate

The protocol you implement to respond to changes to a screen-recording user interface.

