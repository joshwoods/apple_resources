

- ScreenCaptureKit
-  SCWindow 

Class

# SCWindow

An instance that represents an onscreen window.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCWindow
```

## Overview

Retrieve the available windows from an instance of SCShareableContent. Select one or more windows to capture and use them to create an instance of SCContentFilter. Apply the filter to an instance of SCStream to limit its output to content matching your criteria.

## Topics

### Identifying windows

var windowID: CGWindowID

The Core Graphics window identifier.

var title: String?

The string that displays in a window’s title bar.

var owningApplication: SCRunningApplication?

The app that owns the window.

var windowLayer: Int

The layer of the window relative to other windows.

### Accessing dimensions

var frame: CGRect

A rectangle the represents the frame of the window within a display.

### Determining visibility

var isOnScreen: Bool

A Boolean value that indicates whether the window is on screen.

var isActive: Bool

A Boolean value that indicates if the window is currently streaming.

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

### Shareable content

class SCShareableContent

An instance that represents a set of displays, apps, and windows that your app can capture.

class SCShareableContentInfo

An instance that provides information for the content in a given stream.

enum SCShareableContentStyle

The style of content presented in a stream.

class SCDisplay

An instance that represents a display device.

class SCRunningApplication

An instance that represents an app running on a device.

