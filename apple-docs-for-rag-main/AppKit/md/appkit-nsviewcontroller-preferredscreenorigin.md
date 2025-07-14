

- AppKit
- NSViewController
-  preferredScreenOrigin 

Instance Property

# preferredScreenOrigin

For a view controller that is part of an app extension, the preferred screen origin.

macOS 10.10+

``` source
@MainActor
var preferredScreenOrigin: NSPoint { get set }
```

## Discussion

Set this property to position the lower-left corner of the app extension’s primary view in screen space. To specify the desired primary view size for an app extension’s view controller, use the preferredContentSize property.

## See Also

### Related Documentation

var preferredContentSize: NSSize

The desired size of the view controller’s view, in screen units.

### Configuring an App Extension View Controller

var extensionContext: NSExtensionContext?

For a view controller that is part of an app extension, the app extension context.

var preferredMaximumSize: NSSize

For a view controller that is part of an app extension, the largest allowable size for the app extension’s primary view, in screen units.

var preferredMinimumSize: NSSize

For a view controller that is part of an app extension, the smallest allowable size for the app extension’s primary view, in screen units.

func viewWillTransition(to: NSSize)

For a view controller that is part of an app extension, called when its view is about to be resized.

var sourceItemView: NSView?

