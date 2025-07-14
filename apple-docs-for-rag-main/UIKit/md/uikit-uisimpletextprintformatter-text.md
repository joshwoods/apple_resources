

- UIKit
- UISimpleTextPrintFormatter
-  text 

Instance Property

# text

A string of plain text.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var text: String? { get set }
```

## Discussion

You cannot change the value of this property once drawing begins for a print job. The delegate method printInteractionControllerWillStartJob(_:) is called immediately before the formatting is set for the job.

Assigning a value to this property replaces the value in the attributedText property with the same string data, albeit without any inherent style attributes. Instead, the print formatter styles the new string using the text attribute properties of this class.

## See Also

### Related Documentation

init(text: String)

Returns a simple-text print formatter initialized with plain text.

### Getting and setting the text

var attributedText: NSAttributedString?

A string of attributed text.

