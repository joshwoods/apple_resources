

- AVFoundation
-  AVMediaExtensionProperties 

Class

# AVMediaExtensionProperties

An object that describes a Media Extension.

macOS 15.0+

``` source
class AVMediaExtensionProperties
```

## Topics

### Inspecting the extension

var extensionName: String

The name of the Media Extension.

var containingBundleName: String

The name of the containing app bundle.

var extensionURL: URL

The file URL of the Media Extension bundle.

var containingBundleURL: URL

The file URL of the host application for the Media Extension.

### Instance Properties

var extensionIdentifier: String

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Accessing Media Extension Properties

var mediaExtensionProperties: AVMediaExtensionProperties?

The properties of the media extension format reader that decodes the asset.

