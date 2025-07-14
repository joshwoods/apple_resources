

- AppKit
- NSGraphicsContext
-  isDrawingToScreen 

Instance Property

# isDrawingToScreen

A Boolean value that indicates whether the drawing destination is the screen.

macOS

``` source
var isDrawingToScreen: Bool { get }
```

## Discussion

true if the drawing destination is the screen. If the value of the property is false may mean that the drawing destination is a printer, but the destination may also be a PDF or EPS file. You can call attributes to see if additional information is available about the drawing destination.

## See Also

### Testing the Drawing Destination

class func currentContextDrawingToScreen() -> Bool

Returns a Boolean value that indicates whether the current context is drawing to the screen.

