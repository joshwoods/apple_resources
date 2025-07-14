

- UIKit
- UILabel
-  shadowOffset 

Instance Property

# shadowOffset

The shadow offset, in points, for the text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shadowOffset: CGSize { get set }
```

## Discussion

The shadow color must be not be `nil` for this property to have any effect. The default offset size is `(0, -1)`, which indicates a shadow one point above the text. A label draws its text shadows with the specified offset and color and no blurring.

## See Also

### Drawing a shadow

var shadowColor: UIColor?

The shadow color of the text.

