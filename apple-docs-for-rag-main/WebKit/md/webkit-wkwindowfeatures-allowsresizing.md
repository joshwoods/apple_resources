

- WebKit
- WKWindowFeatures
-  allowsResizing 

Instance Property

# allowsResizing

A Boolean value that indicates whether to make the containing window window resizable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var allowsResizing: NSNumber? { get }
```

## Discussion

If the webpage didn’t request a resizable window, this property is `nil`.

## See Also

### Inspecting Window Position and Dimensions

var height: NSNumber?

The requested height of the containing window.

var width: NSNumber?

The requested width of the containing window.

var x: NSNumber?

The requested x-coordinate of the containing window.

var y: NSNumber?

The requested y-coordinate of the containing window.

