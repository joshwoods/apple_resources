

- UIKit
- UIMarkupTextPrintFormatter
-  init(markupText:) 

Initializer

# init(markupText:)

Returns a markup-text print formatter initialized with an HTML string.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(markupText: String)
```

## Parameters 

`markupText`  

A string of HTML markup text or `nil` if you want to add the markup text later.

## Return Value

An instance of `UIMarkupTextPrintFormatter` or `nil` if the object could not be created.

## See Also

### Related Documentation

var markupText: String?

The HTML markup text for the print formatter.

