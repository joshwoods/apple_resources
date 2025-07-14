

- AppKit
- NSPageController
-  selectedViewController 

Instance Property

# selectedViewController

The view controller associated with the selected object..

macOS 10.8+

``` source
@MainActor
var selectedViewController: NSViewController? { get }
```

## Discussion

May be `nil` if not using view controllers.

This property is only relevant in book mode. See Book Mode (View Controller Mode) for details.

