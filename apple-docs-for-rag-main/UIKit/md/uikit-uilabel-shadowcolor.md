

- UIKit
- UILabel
-  shadowColor 

Instance Property

# shadowColor

The shadow color of the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shadowColor: UIColor? { get set }
```

## Discussion

The default value for this property is `nil`, which indicates that the text has no shadow. In addition to this property, you may also want to change the default shadow offset by modifying the shadowOffset property. A label draws its text shadows with the specified offset and color and no blurring.

## See Also

### Drawing a shadow

var shadowOffset: CGSize

The shadow offset, in points, for the text.

