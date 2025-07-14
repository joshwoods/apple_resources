

- AppKit
- NSView
- NSView.Invalidations
- NSView.Invalidations.Display
-  init() 

Initializer

# init()

Creates the invalidation type.

macOS 12.0+Swift 5.1+

``` source
init()
```

## See Also

### Creating the invalidation type

func display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

