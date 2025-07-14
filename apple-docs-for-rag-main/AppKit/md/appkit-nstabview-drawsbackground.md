

- AppKit
- NSTabView
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value that indicates if the tab view draws a background color when its type is `NSNoTabsNoBorder`.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the tab view draws a background color when the its type is `NSNoTabsNoBorder`, otherwise it does not. If the tab view has a bezeled border or a line border, the appropriate background for that border is used. The default value of this property is true.

## See Also

### Related Documentation

var tabViewType: NSTabView.TabType

The tab type to display the tabs.

