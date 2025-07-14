

- UIKit
- UISimpleTextPrintFormatter
-  attributedText 

Instance Property

# attributedText

A string of attributed text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var attributedText: NSAttributedString? { get set }
```

## Discussion

You cannot change the value of this property once drawing begins for a print job. The delegate method printInteractionControllerWillStartJob(_:) is called immediately before the formatting is set for the job.

Assigning a value to this property also replaces the value in the text property with the same string data, albeit without any formatting information.

## See Also

### Related Documentation

init(attributedText: NSAttributedString)

Returns a simple-text print formatter initialized with attributed text.

### Getting and setting the text

var text: String?

A string of plain text.

