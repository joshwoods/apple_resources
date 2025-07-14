

- UIKit
- UISimpleTextPrintFormatter
-  color 

Instance Property

# color

The color of the printed text.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var color: UIColor? { get set }
```

## Discussion

If the value of this property is `nil` (the default), UIKit uses a black color when printing.

## See Also

### Text attributes for printed content

var font: UIFont?

The font of the printed text.

var textAlignment: NSTextAlignment

The alignment of the printed text.

