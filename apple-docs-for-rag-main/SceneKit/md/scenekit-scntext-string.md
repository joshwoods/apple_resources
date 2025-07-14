

- SceneKit
- SCNText
-  string 

Instance Property

# string

The string object whose text the geometry represents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var string: Any? { get set }
```

## Discussion

You can supply text as an NSString or NSAttributedString object. When you use an NSString object, the text geometry’s properties determine the style of the entire body of text. You can use an NSAttributedString object to provide a body of text containing multiple styles, in which case the text geometry’s properties define the default style for portions of the string without style attributes.

The default value of this property is `nil`, which creates an empty text geometry.

## See Also

### Managing the Geometry’s Text Content

var font: UIFont!

The font that SceneKit uses to create geometry from the text.

