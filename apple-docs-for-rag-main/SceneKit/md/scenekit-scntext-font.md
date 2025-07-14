

- SceneKit
- SCNText
-  font 

Instance Property

# font

The font that SceneKit uses to create geometry from the text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
var font: NSFont! { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var font: UIFont! { get set }
```

## Discussion

If the text geometry’s string property is an NSString object, SceneKit uses this font to render the entire text. If the string property is an an NSAttributedString object, SceneKit uses this font for any portions of the string not containing style attributes.

The default font is Helvetica 36 point.

## See Also

### Managing the Geometry’s Text Content

var string: Any?

The string object whose text the geometry represents.

