

- SwiftUI
- NSHostingView
-  safeAreaRegions 

Instance Property

# safeAreaRegions

The safe area regions that this view controller adds to its view.

macOS 13.3+

``` source
@MainActor @preconcurrency
var safeAreaRegions: SafeAreaRegions { get set }
```

## Discussion

The default value is `SafeAreaRegions.all`.

## See Also

### Configuring the view layout behavior

class var requiresConstraintBasedLayout: Bool

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

var isFlipped: Bool

var layerContentsRedrawPolicy: NSView.LayerContentsRedrawPolicy

func updateConstraints()

func layout()

