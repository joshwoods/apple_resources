

- AVFoundation
- AVURLAsset
-  mediaExtensionProperties 

Instance Property

# mediaExtensionProperties

The properties of the media extension format reader that decodes the asset.

macOS 15.0+

``` source
var mediaExtensionProperties: AVMediaExtensionProperties? { get }
```

## Discussion

If the system decodes the asset using a MediaExtension format reader, the property value contains a valid object that describes the extension. Otherwise, this property value is `nil`.

## See Also

### Accessing Media Extension Properties

class AVMediaExtensionProperties

An object that describes a Media Extension.

