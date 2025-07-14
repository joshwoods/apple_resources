

- AppKit
- NSWindowTab
-  title 

Instance Property

# title

The title for the window tab.

macOS 10.13+

``` source
var title: String! { get set }
```

## Discussion

The title displays within the window tab when the associated window is part of a tabbing group.

By default, the title of the window tab follows the title of its associated window, but it may be customized using the title property. If the title has been customized, setting the title property to Nil causes it to follow the window’s title again.

## See Also

### Customizing the Title

var attributedTitle: NSAttributedString?

The title for the window tab, specified as an attributed string.

