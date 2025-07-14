

- AppKit
- NSGraphicsContext
-  currentContextDrawingToScreen() 

Type Method

# currentContextDrawingToScreen()

Returns a Boolean value that indicates whether the current context is drawing to the screen.

macOS

``` source
class func currentContextDrawingToScreen() -> Bool
```

## Return Value

true if the current context is drawing to the screen, otherwise false.

## Discussion

This convenience method is equivalent to sending isDrawingToScreen to the result of current.

## See Also

### Testing the Drawing Destination

var isDrawingToScreen: Bool

A Boolean value that indicates whether the drawing destination is the screen.

