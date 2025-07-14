

- AppKit
- NSViewController
-  viewWillTransition(to:) 

Instance Method

# viewWillTransition(to:)

For a view controller that is part of an app extension, called when its view is about to be resized.

macOS 10.10+

``` source
@MainActor
func viewWillTransition(to newSize: NSSize)
```

## Parameters 

`newSize`  

The new size for the view controller’s view.

## Discussion

Override this method if you want to change layout in response to the change in size, potentially in an animated way.

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

var sourceItemView: NSView?

