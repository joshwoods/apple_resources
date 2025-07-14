

- AppKit
- NSView
-  init(frame:) 

Initializer

# init(frame:)

Initializes and returns a newly allocated `NSView` object with a specified frame rectangle.

macOS

``` source
@MainActor
init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame rectangle for the created view object.

## Return Value

An initialized view or `nil` if AppKit couldn’t create the object.

## Discussion

Insert the view into your window’s view hieararchy before you can do anything with it. This method is the designated initializer for the NSView class.

## See Also

### Related Documentation

func addSubview(NSView, positioned: NSWindow.OrderingMode, relativeTo: NSView?)

Inserts a view among the view’s subviews so it’s displayed immediately above or below another view.

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func addSubview(NSView)

Adds a view to the view’s subviews so it’s displayed above its siblings.

View Programming Guide

### Creating a view object

init?(coder: NSCoder)

Initializes a view using from data in the specified coder object.

func prepareForReuse()

Restores the view to an initial state so that it can be reused.

