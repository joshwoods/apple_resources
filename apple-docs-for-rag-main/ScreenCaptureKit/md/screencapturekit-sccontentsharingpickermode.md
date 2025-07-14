

- ScreenCaptureKit
-  SCContentSharingPickerMode 

Structure

# SCContentSharingPickerMode

Available modes for selecting streaming content from a picker presented by the operating system.

Mac Catalyst 18.2+macOS 14.0+

``` source
struct SCContentSharingPickerMode
```

## Topics

### Initializers

init(rawValue: UInt)

Initializes a sharing-picker mode.

### Picker selection modes

static var multipleApplications: SCContentSharingPickerMode

The mode allowing the selection of multiple applications through the presented picker.

static var multipleWindows: SCContentSharingPickerMode

The mode allowing the selection of multiple windows through the presented picker.

static var singleApplication: SCContentSharingPickerMode

The mode allowing the selection of a single application through the presented picker.

static var singleDisplay: SCContentSharingPickerMode

The mode allowing the selection of a single display through the presented picker.

static var singleWindow: SCContentSharingPickerMode

The mode allowing the selection of a single window through the presented picker.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### System content-sharing picker

class SCContentSharingPicker

An instance of a picker presented by the operating system for managing frame-capture streams.

struct SCContentSharingPickerConfiguration

An instance for configuring the system content-sharing picker.

protocol SCContentSharingPickerObserver

An observer protocol your app implements to receive messages from the operating system’s content picker.

