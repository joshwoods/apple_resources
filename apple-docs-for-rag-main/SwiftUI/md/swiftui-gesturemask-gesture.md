

- SwiftUI
- GestureMask
-  gesture 

Type Property

# gesture

Enable the added gesture but disable all gestures in the subview hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let gesture: GestureMask
```

## See Also

### Getting gesture options

static let all: GestureMask

Enable both the added gesture as well as all other gestures on the view and its subviews.

static let subviews: GestureMask

Enable all gestures in the subview hierarchy but disable the added gesture.

static let none: GestureMask

Disable all gestures in the subview hierarchy, including the added gesture.

