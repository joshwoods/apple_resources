

- AppKit
- NSPopover
-  contentViewController 

Instance Property

# contentViewController

The view controller that manages the content of the popover.

macOS 10.7+

``` source
@IBOutlet @MainActor
var contentViewController: NSViewController? { get set }
```

## Discussion

You must set the content view controller of the popover before the popover is shown. Changes to the popover’s content view controller while the popover is shown will cause the popover to animate if the animates property is true.

The default value is `nil`.

