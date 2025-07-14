

- UIKit
- UISimpleTextPrintFormatter
-  font 

Instance Property

# font

The font of the printed text.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var font: UIFont? { get set }
```

## Discussion

If the value of this property is `nil` (the default), UIKit uses the standard system font, 12 points.

## See Also

### Text attributes for printed content

var color: UIColor?

The color of the printed text.

var textAlignment: NSTextAlignment

The alignment of the printed text.

