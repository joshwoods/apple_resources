

- Video Toolbox
- VTExtensionPropertiesKey
-  containingBundleName 

Type Property

# containingBundleName

A dictionary key for the extension host application localized name.

macOS 15.0+

``` source
static let containingBundleName: VTExtensionPropertiesKey
```

## Discussion

This key points to a `CFStringRef` value with the localized name of the application hosting the extension.

## See Also

### Keys

static let containingBundleURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension host application.

static let extensionIdentifier: VTExtensionPropertiesKey

A dictionary key for the video decoder extension identifier.

static let extensionName: VTExtensionPropertiesKey

A dictionary key for the localized extension name.

static let extensionURL: VTExtensionPropertiesKey

A dictionary key for the URL of the extension.

