

- ScreenCaptureKit
-  SCContentSharingPickerObserver 

Protocol

# SCContentSharingPickerObserver

An observer protocol your app implements to receive messages from the operating system’s content picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
protocol SCContentSharingPickerObserver : NSObjectProtocol
```

## Topics

### Observing events

func contentSharingPicker(SCContentSharingPicker, didCancelFor: SCStream?)

Tells the observer that a sharing picker canceled selection for a stream.

**Required**

func contentSharingPicker(SCContentSharingPicker, didUpdateWith: SCContentFilter, for: SCStream?)

Tells the observer that a sharing picker updated the content filter for a stream.

**Required**

### Observing errors

func contentSharingPickerStartDidFailWithError(any Error)

Tells the observer that a sharing picker was unable to start.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### System content-sharing picker

class SCContentSharingPicker

An instance of a picker presented by the operating system for managing frame-capture streams.

struct SCContentSharingPickerConfiguration

An instance for configuring the system content-sharing picker.

struct SCContentSharingPickerMode

Available modes for selecting streaming content from a picker presented by the operating system.

