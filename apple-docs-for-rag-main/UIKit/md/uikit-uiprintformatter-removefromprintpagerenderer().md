

- UIKit
- UIPrintFormatter
-  removeFromPrintPageRenderer() 

Instance Method

# removeFromPrintPageRenderer()

Removes the print formatter from the page renderer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func removeFromPrintPageRenderer()
```

## Discussion

A print formatter is typically associated with a pages of a UIPrintPageRenderer object through the addPrintFormatter(_:startingAtPageAt:) method.

## See Also

### Communicating with the page renderer

var printPageRenderer: UIPrintPageRenderer?

Returns the page renderer for the print formatter.

