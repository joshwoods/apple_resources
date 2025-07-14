

- WebKit
- WKWindowFeatures
-  height 

Instance Property

# height

The requested height of the containing window.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var height: NSNumber? { get }
```

## Discussion

The object in this property contains a CGFloat value. If the webpage didn’t request a specific window height, this property is `nil`.

## See Also

### Inspecting Window Position and Dimensions

var allowsResizing: NSNumber?

A Boolean value that indicates whether to make the containing window window resizable.

var width: NSNumber?

The requested width of the containing window.

var x: NSNumber?

The requested x-coordinate of the containing window.

var y: NSNumber?

The requested y-coordinate of the containing window.

