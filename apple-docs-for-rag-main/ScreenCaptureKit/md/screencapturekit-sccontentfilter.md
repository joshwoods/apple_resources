

- ScreenCaptureKit
-  SCContentFilter 

Class

# SCContentFilter

An instance that filters the content a stream captures.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCContentFilter
```

## Overview

Use a content filter to limit an SCStream object’s output to only that matching your filter criteria. Retrieve the displays, apps, and windows that your app can capture from an instance of SCShareableContent.

## Topics

### Creating a filter

init(desktopIndependentWindow: SCWindow)

Creates a filter that captures only the specified window.

init(display: SCDisplay, including: [SCWindow])

Creates a filter that captures only specific windows from a display.

init(display: SCDisplay, excludingWindows: [SCWindow])

Creates a filter that captures the contents of a display, excluding the specified windows.

init(display: SCDisplay, including: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, including only windows of the specified apps.

init(display: SCDisplay, excludingApplications: [SCRunningApplication], exceptingWindows: [SCWindow])

Creates a filter that captures a display, excluding windows of the specified apps.

### Filter properties

var contentRect: CGRect

The size and location of the content to filter, in screen points.

var pointPixelScale: Float

The scaling factor used to translate screen points into pixels.

var streamType: SCStreamType

The type of the streaming content.

Deprecated

enum SCStreamType

The display type of the presented stream.

Deprecated

var style: SCShareableContentStyle

The display style of the sharable content.

### Instance Properties

var includeMenuBar: Bool

var includedApplications: [SCRunningApplication]

var includedDisplays: [SCDisplay]

var includedWindows: [SCWindow]

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

### Content capture

class SCStream

An instance that represents a stream of shareable content.

class SCStreamConfiguration

An instance that provides the output configuration for a stream.

protocol SCStreamDelegate

A delegate protocol your app implements to respond to stream events.

class SCScreenshotManager

An instance for the capture of single frames from a stream.

