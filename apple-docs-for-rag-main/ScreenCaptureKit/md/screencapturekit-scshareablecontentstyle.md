

- ScreenCaptureKit
-  SCShareableContentStyle 

Enumeration

# SCShareableContentStyle

The style of content presented in a stream.

Mac Catalyst 18.2+macOS 12.3+

``` source
enum SCShareableContentStyle
```

## Topics

### Content styles

case application

The stream is currently presenting one or more applications.

case display

The stream is currently presenting a complete display.

case none

The stream isn’t currently presenting any content.

case window

The stream is currently presenting one or more windows.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Shareable content

class SCShareableContent

An instance that represents a set of displays, apps, and windows that your app can capture.

class SCShareableContentInfo

An instance that provides information for the content in a given stream.

class SCDisplay

An instance that represents a display device.

class SCRunningApplication

An instance that represents an app running on a device.

class SCWindow

An instance that represents an onscreen window.

