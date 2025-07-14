

- AppKit
-  NSTextViewportLayoutControllerDelegate 

Protocol

# NSTextViewportLayoutControllerDelegate

Optional methods that delegates implement to respond to viewport layout changes.

macOS 12.0+

``` source
protocol NSTextViewportLayoutControllerDelegate : NSObjectProtocol
```

## Topics

### Responding to changes in the viewport

func textViewportLayoutController(NSTextViewportLayoutController, configureRenderingSurfaceFor: NSTextLayoutFragment)

The method the framework calls when the layout controller lays out a text layout fragment in the UI.

**Required**

func textViewportLayoutControllerDidLayout(NSTextViewportLayoutController)

The method the framework calls when the text viewport layout controller finishes its layout process.

func textViewportLayoutControllerWillLayout(NSTextViewportLayoutController)

The method the framework calls before the text viewport layout controller starts its layout process.

func viewportBounds(for: NSTextViewportLayoutController) -> CGRect

Returns the current viewport, which is the view visible bounds plus the overdraw area.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to changes in viewport layout

var delegate: (any NSTextViewportLayoutControllerDelegate)?

The delegate for the text layout manager object.

