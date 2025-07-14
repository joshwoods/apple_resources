

- AppKit
- NSWindowTab
-  attributedTitle 

Instance Property

# attributedTitle

The title for the window tab, specified as an attributed string.

macOS 10.13+

``` source
@NSCopying
var attributedTitle: NSAttributedString? { get set }
```

## Discussion

If you provide an attributed title, the window tab uses all of the attributes that are explicitly provided in the attributed string. Attributes that are left unspecified, including the font and foreground color, are automatically filled in using default values appropriate for the window tab.

If the attributedTitle property is nil, the window tab uses the title property instead. The default value is Nil.

## See Also

### Customizing the Title

var title: String!

The title for the window tab.

