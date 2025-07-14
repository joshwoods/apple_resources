

- AppKit
- NSViewController
-  view 

Instance Property

# view

The view controller’s primary view.

macOS 10.5+

``` source
@IBOutlet @MainActor
var view: NSView { get set }
```

## Discussion

If this property’s value is not already set when you access it, the view controller invokes the loadView() method. That method, in turn, sets the view from the nib file identified by the view controller’s nibName and nibBundle properties.

If you want to set a view controller’s view directly, set this property’s value immediately after creating the view controller.

## See Also

### View Properties

var title: String?

The localized title of the receiver’s primary view.

