

- UIKit
- UIGraphicsPDFRendererContext
-  pdfContextBounds 

Instance Property

# pdfContextBounds

The bounds of the PDF context for the current page.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var pdfContextBounds: CGRect { get }
```

## Discussion

This value represents the bounds provided to the beginPage(withBounds:pageInfo:) method that created the current page. If the current page was created using the beginPage() method, the bounds are equal to those provided at the initialization of the PDF renderer.

