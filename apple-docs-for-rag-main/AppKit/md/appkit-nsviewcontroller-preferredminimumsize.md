

- AppKit
- NSViewController
-  preferredMinimumSize 

Instance Property

# preferredMinimumSize

For a view controller that is part of an app extension, the smallest allowable size for the app extension’s primary view, in screen units.

macOS 10.10+

``` source
@MainActor
var preferredMinimumSize: NSSize { get }
```

## Discussion

An app extension should return the minimum dimensions its primary view can accommodate, based on the items the app extension has been sent. By default, the value of this property is a small but non-empty size.

## See Also

### Related Documentation

var preferredContentSize: NSSize

The desired size of the view controller’s view, in screen units.

### Configuring an App Extension View Controller

var extensionContext: NSExtensionContext?

For a view controller that is part of an app extension, the app extension context.

var preferredScreenOrigin: NSPoint

For a view controller that is part of an app extension, the preferred screen origin.

var preferredMaximumSize: NSSize

For a view controller that is part of an app extension, the largest allowable size for the app extension’s primary view, in screen units.

func viewWillTransition(to: NSSize)

For a view controller that is part of an app extension, called when its view is about to be resized.

var sourceItemView: NSView?

