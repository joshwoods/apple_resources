

- Video Toolbox
- VTExtensionPropertiesKey
-  extensionIdentifier 

Type Property

# extensionIdentifier

A dictionary key for the video decoder extension identifier.

macOS 15.0+

``` source
static let extensionIdentifier: VTExtensionPropertiesKey
```

## Discussion

This key points to a `CFStringRef` value with the extension identifier, corresponding to the ClassImplementationID value from the EXAppExtensionAttributes dictionary in the Info.plist file.

## See Also

### Keys

static let containingBundleName: VTExtensionPropertiesKey

A dictionary key for the extension host application localized name.

static let containingBundleURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension host application.

static let extensionName: VTExtensionPropertiesKey

A dictionary key for the localized extension name.

static let extensionURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension.

