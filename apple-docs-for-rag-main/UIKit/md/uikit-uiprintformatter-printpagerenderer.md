

- UIKit
- UIPrintFormatter
-  printPageRenderer 

Instance Property

# printPageRenderer

Returns the page renderer for the print formatter.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var printPageRenderer: UIPrintPageRenderer? { get }
```

## Discussion

If the receiving print formatter was not added to a page renderer—that is, it was assigned to the printFormatter property of the UIPrintInteractionController class—the value returned is `nil`.

## See Also

### Communicating with the page renderer

func removeFromPrintPageRenderer()

Removes the print formatter from the page renderer.

