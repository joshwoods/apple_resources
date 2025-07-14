

- ScreenCaptureKit
-  SCContentSharingPicker 

Class

# SCContentSharingPicker

An instance of a picker presented by the operating system for managing frame-capture streams.

Mac Catalyst 18.2+macOS 14.0+

``` source
class SCContentSharingPicker
```

## Overview

Important

Avoid creating your own sharing picker. Use the picker provided by the shared static property.

## Topics

### Shared system picker

class var shared: SCContentSharingPicker

The system-provided picker UI instance for capturing display and audio content from someone’s Mac.

### Picker availability

var isActive: Bool

A Boolean value that indicates if the picker is active.

### Stream configuration

func setConfiguration(SCContentSharingPickerConfiguration?, for: SCStream)

Sets the configuration for the content capture picker for a capture stream, providing allowed selection modes and content excluded from selection.

var configuration: SCContentSharingPickerConfiguration?

Sets the configuration for the content capture picker for all streams, providing allowed selection modes and content excluded from selection.

var defaultConfiguration: SCContentSharingPickerConfiguration

The default configuration to use for the content capture picker.

var maximumStreamCount: Int?

The maximum number of streams the content capture picker allows.

### Manage observers

func add(any SCContentSharingPickerObserver)

Adds an observer instance to notify of changes in the content-sharing picker.

func remove(any SCContentSharingPickerObserver)

Removes an observer instance from the content-sharing picker.

### Picker display

func present()

Displays the picker with no active selection for capture.

func present(for: SCStream)

Displays the picker with an already running capture stream.

func present(using: SCShareableContentStyle)

Displays the picker for a single type of capture selection.

func present(for: SCStream, using: SCShareableContentStyle)

Displays the picker with an existing capture stream, allowing for a single type of capture selection.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### System content-sharing picker

struct SCContentSharingPickerConfiguration

An instance for configuring the system content-sharing picker.

struct SCContentSharingPickerMode

Available modes for selecting streaming content from a picker presented by the operating system.

protocol SCContentSharingPickerObserver

An observer protocol your app implements to receive messages from the operating system’s content picker.

