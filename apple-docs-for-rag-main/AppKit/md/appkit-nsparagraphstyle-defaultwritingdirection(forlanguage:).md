

- AppKit
- NSParagraphStyle
-  defaultWritingDirection(forLanguage:) 

Type Method

# defaultWritingDirection(forLanguage:)

Returns the default writing direction for the specified language.

macOS 10.0+

``` source
class func defaultWritingDirection(forLanguage languageName: String?) -> NSWritingDirection
```

## Parameters 

`languageName`  

The language specified in ISO language region format. Can be `nil` to return a default writing direction derived from the user’s defaults database.

## Return Value

The default writing direction.

## See Also

### Determining writing direction

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

enum NSWritingDirection

Constants that specify the writing direction.

