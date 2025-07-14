

- AppKit
- NSWindow
-  contentViewController 

Instance Property

# contentViewController

The main content view controller for the window.

macOS 10.10+

``` source
@MainActor
var contentViewController: NSViewController? { get set }
```

## Discussion

The value of this property provides the content view of the window. Setting this value removes the existing value of contentView and makes the `contentViewController.view` the main content view for the window. By default, the value of this property is `nil`.

The content view controller controls only the contentView object, and not the title of the window. The window title can easily be bound to the contentViewController object using code such as: `[window bind:NSTitleBinding toObject:contentViewController withKeyPath:@"title" options:nil]`. Setting contentViewController causes the window to resize based on the current size of the contentViewController; to restrict the size of the window, use Auto Layout (note that the value of this property is encoded in the NIB). Directly assigning a contentView value clears out the root view controller.

## See Also

### Related Documentation

convenience init(contentViewController: NSViewController)

Creates a titled window that contains the specified content view controller.

### Configuring the Window’s Content

var contentView: NSView?

The window’s content view, the highest accessible view object in the window’s view hierarchy.

