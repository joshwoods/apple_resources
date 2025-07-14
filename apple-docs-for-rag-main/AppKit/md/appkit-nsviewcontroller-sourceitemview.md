

- AppKit
- NSViewController
-  sourceItemView 

Instance Property

# sourceItemView

macOS 10.10+

``` source
@IBOutlet @MainActor
var sourceItemView: NSView? { get set }
```

## See Also

### Configuring an App Extension View Controller

var extensionContext: NSExtensionContext?

For a view controller that is part of an app extension, the app extension context.

var preferredScreenOrigin: NSPoint

For a view controller that is part of an app extension, the preferred screen origin.

var preferredMaximumSize: NSSize

For a view controller that is part of an app extension, the largest allowable size for the app extension’s primary view, in screen units.

var preferredMinimumSize: NSSize

For a view controller that is part of an app extension, the smallest allowable size for the app extension’s primary view, in screen units.

func viewWillTransition(to: NSSize)

For a view controller that is part of an app extension, called when its view is about to be resized.

