

- AVFoundation
- AVMediaExtensionProperties
-  extensionName 

Instance Property

# extensionName

The name of the Media Extension.

macOS 15.0+

``` source
var extensionName: String { get }
```

## Discussion

This value corresponds to the extension’s CFBundleDisplayName.

## See Also

### Inspecting the extension

var containingBundleName: String

The name of the containing app bundle.

var extensionURL: URL

The file URL of the Media Extension bundle.

var containingBundleURL: URL

The file URL of the host application for the Media Extension.

