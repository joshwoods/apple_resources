

- AppKit
- NSWindowTab
-  toolTip 

Instance Property

# toolTip

The tooltip for this window tab.

macOS 10.13+

``` source
var toolTip: String! { get set }
```

## Discussion

By default, the window tab’s tooltip displays its title string. Once customized, setting the toolTip property to Nil causes it to follow the title property again.

