

- UIKit
- UIMarkupTextPrintFormatter
-  markupText 

Instance Property

# markupText

The HTML markup text for the print formatter.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var markupText: String? { get set }
```

## Discussion

When drawing begins for the print job, you cannot change the value of this property. The delegate method printInteractionControllerWillStartJob(_:) is called immediately before the formatting is set for the job.

## See Also

### Related Documentation

init(markupText: String)

Returns a markup-text print formatter initialized with an HTML string.

