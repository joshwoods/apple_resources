

- ScreenCaptureKit
-  SCRunningApplication 

Class

# SCRunningApplication

An instance that represents an app running on a device.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCRunningApplication
```

## Overview

Retrieve the available apps from an instance of SCShareableContent. Select one or more apps to capture and use them to create an instance of SCContentFilter. Apply the filter to an instance of SCStream to limit its output to content matching your criteria.

## Topics

### Inspecting an app

var processID: pid_t

The system process identifier of the app.

var bundleIdentifier: String

The unique bundle identifier of the app.

var applicationName: String

The display name of the app.

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

class SCWindow

An instance that represents an onscreen window.

