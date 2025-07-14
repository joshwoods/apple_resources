

- UIKit
- UISimpleTextPrintFormatter
-  init(text:) 

Initializer

# init(text:)

Returns a simple-text print formatter initialized with plain text.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(text: String)
```

## Parameters 

`text`  

A string of plain text or `nil` if you intend to assign the text later.

## Return Value

An initialized instance of `UISimpleTextPrintFormatter` or `nil` if the object could not be created.

## See Also

### Related Documentation

var text: String?

A string of plain text.

### Creating a simple-text print formatter

init(attributedText: NSAttributedString)

Returns a simple-text print formatter initialized with attributed text.

