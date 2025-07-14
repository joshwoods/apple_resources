

- UIKit
- UISimpleTextPrintFormatter
-  init(attributedText:) 

Initializer

# init(attributedText:)

Returns a simple-text print formatter initialized with attributed text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(attributedText: NSAttributedString)
```

## Parameters 

`attributedText`  

A string of attributed text or `nil` if you intend to assign the text later.

## Return Value

An initialized instance of `UISimpleTextPrintFormatter` or `nil` if the object could not be created.

## See Also

### Related Documentation

var attributedText: NSAttributedString?

A string of attributed text.

### Creating a simple-text print formatter

init(text: String)

Returns a simple-text print formatter initialized with plain text.

