

- AppKit
- NSRulerView
-  init(scrollView:orientation:) 

Initializer

# init(scrollView:orientation:)

Initializes a newly allocated NSRulerView to have `orientation` (`NSHorizontalRuler` or `NSVerticalRuler`) within `aScrollView`.

macOS

``` source
@MainActor
init(
    scrollView: NSScrollView?,
    orientation: NSRulerView.Orientation
)
```

## Discussion

The new ruler view displays the user’s preferred measurement units and has no client, markers, or accessory view. Unlike most subclasses of NSView, no initial frame rectangle is given for NSRulerView; its containing NSScrollView adjusts its frame rectangle as needed.

This method is the designated initializer for the NSRulerView class. Returns an initialized object.

## See Also

### Related Documentation

Ruler and Paragraph Style Programming Topics

### Creating a Ruler View

init(coder: NSCoder)

