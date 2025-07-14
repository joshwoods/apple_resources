

- AppKit
- NSWindow
-  init(contentViewController:) 

Initializer

# init(contentViewController:)

Creates a titled window that contains the specified content view controller.

macOS 10.10+

``` source
@MainActor
convenience init(contentViewController: NSViewController)
```

## Parameters 

`contentViewController`  

The view controller that provides the main content view for the window. The window’s contentView property is set to ``` contentViewController``.view ```.

## Return Value

A window with the content view controller set to the passed-in view controller object.

## Discussion

This method creates a basic window object that is titled, closable, resizable, and miniaturizable. By default, the window’s title is automatically bound to the title of `contentViewController`. You can control the size of the window by using Auto Layout and applying size constraints to the view or its subviews. The initial size of the window is set to the initial size of contentView (that is, the size of ``` contentViewController``.view ```). The newly created window has isReleasedWhenClosed set to false, and it must be explicitly retained to keep the window instance alive.

## See Also

### Related Documentation

Window Programming Guide

var contentViewController: NSViewController?

The main content view controller for the window.

### Creating a Window

init(contentRect: NSRect, styleMask: NSWindow.StyleMask, backing: NSWindow.BackingStoreType, defer: Bool)

Initializes the window with the specified values.

convenience init(contentRect: NSRect, styleMask: NSWindow.StyleMask, backing: NSWindow.BackingStoreType, defer: Bool, screen: NSScreen?)

Initializes an allocated window with the specified values.

