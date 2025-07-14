

- AppKit
- NSFont
-  fontName 

Instance Property

# fontName

The full name of the font, as used in PostScript language code—for example, “Times-Roman” or “Helvetica-Oblique.”

macOS

``` source
var fontName: String { get }
```

## Discussion

The value in this property is intended for an application’s internal usage and not for display. To get a name that you can display to the user, use the displayName property instead.

## See Also

### Getting Font Names

var displayName: String?

The name of the font, including family and face names, to use when displaying the font information to the user.

var familyName: String?

The family name of the font—for example, “Times” or “Helvetica.”

