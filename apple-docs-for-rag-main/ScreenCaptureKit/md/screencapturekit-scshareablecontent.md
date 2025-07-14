

- ScreenCaptureKit
-  SCShareableContent 

Class

# SCShareableContent

An instance that represents a set of displays, apps, and windows that your app can capture.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCShareableContent
```

## Overview

Use the displays, windows, and applications properties to create a SCContentFilter object that specifies what display content to capture. You apply the filter to an instance of SCStream to limit its output to only the content matching your filter.

## Topics

### Retrieving shareable content

class func getWithCompletionHandler((SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that your app can capture.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnly: Bool, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that match your criteria.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyAbove: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are in front of the specified window.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyBelow: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are behind the specified window.

class func info(for: SCContentFilter) -> SCShareableContentInfo

Retrieves any available sharable content information that matches the provided filter.

### Inspecting shareable content

var windows: [SCWindow]

The windows available for capture.

var displays: [SCDisplay]

The displays available for capture.

var applications: [SCRunningApplication]

The apps available for capture.

### Type Methods

class func getCurrentProcessShareableContent(completionHandler: (SCShareableContent?, (any Error)?) -> Void)

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

class SCShareableContentInfo

An instance that provides information for the content in a given stream.

enum SCShareableContentStyle

The style of content presented in a stream.

class SCDisplay

An instance that represents a display device.

class SCRunningApplication

An instance that represents an app running on a device.

class SCWindow

An instance that represents an onscreen window.

