

- UIKit
- NSParagraphStyle
-  baseWritingDirection 

Instance Property

# baseWritingDirection

The base writing direction for the paragraph.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var baseWritingDirection: NSWritingDirection { get }
```

## Discussion

If you the value of this property is NSWritingDirection.natural, the receiver resolves the writing direction to either NSWritingDirection.leftToRight or NSWritingDirection.rightToLeft, depending on the direction for the user’s language preference setting.

## See Also

### Determining writing direction

class func defaultWritingDirection(forLanguage: String?) -> NSWritingDirection

Returns the default writing direction for the specified language.

enum NSWritingDirection

Constants that specify the writing direction.

