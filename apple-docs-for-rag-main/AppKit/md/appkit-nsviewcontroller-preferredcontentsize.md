

- AppKit
- NSViewController
-  preferredContentSize 

Instance Property

# preferredContentSize

The desired size of the view controller’s view, in screen units.

macOS 10.10+

``` source
@MainActor
var preferredContentSize: NSSize { get set }
```

## Discussion

Set this property to express the desired size for a view controller’s view. A parent view controller can consult the value of this property when performing layout.

## See Also

### Related Documentation

var preferredMaximumSize: NSSize

For a view controller that is part of an app extension, the largest allowable size for the app extension’s primary view, in screen units.

var preferredMinimumSize: NSSize

For a view controller that is part of an app extension, the smallest allowable size for the app extension’s primary view, in screen units.

var preferredScreenOrigin: NSPoint

For a view controller that is part of an app extension, the preferred screen origin.

### Managing View Layout

func updateViewConstraints()

Called during Auto Layout constraint updating to enable the view controller to mediate the process.

func viewWillLayout()

Called just before the layout() method of the view controller’s view is called.

func viewDidLayout()

Called immediately after the layout() method of the view controller’s view is called.

