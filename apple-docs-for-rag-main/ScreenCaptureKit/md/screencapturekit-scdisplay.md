

- ScreenCaptureKit
-  SCDisplay 

Class

# SCDisplay

An instance that represents a display device.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCDisplay
```

## Overview

A display object represents a physical display connected to a Mac. Query the display to retrieve its unique identifier and onscreen coordinates.

Retrieve the available displays from an instance of SCShareableContent. Select a display to capture and use it to create an instance of SCContentFilter. Apply the filter to an instance of SCStream to limit its output to content matching your criteria.

## Topics

### Identifying displays

var displayID: CGDirectDisplayID

The Core Graphics display identifier.

### Accessing dimensions

var frame: CGRect

The frame of the display.

var width: Int

The width of the display in points.

var height: Int

The height of the display in points.

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

class SCRunningApplication

An instance that represents an app running on a device.

class SCWindow

An instance that represents an onscreen window.

