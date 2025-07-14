

- Video Toolbox
-  VTExtensionPropertiesKey 

Structure

# VTExtensionPropertiesKey

A key in a Media Extension extension properties dictionary.

macOS 15.0+

``` source
struct VTExtensionPropertiesKey
```

## Topics

### Keys

static let containingBundleName: VTExtensionPropertiesKey

A dictionary key for the extension host application localized name.

static let containingBundleURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension host application.

static let extensionIdentifier: VTExtensionPropertiesKey

A dictionary key for the video decoder extension identifier.

static let extensionName: VTExtensionPropertiesKey

A dictionary key for the localized extension name.

static let extensionURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension.

### Initializers

init(rawValue: CFString)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

