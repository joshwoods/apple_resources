

- AppKit
- NSText
-  alignment 

Instance Property

# alignment

The alignment of all the receiver’s text.

macOS

``` source
@MainActor
var alignment: NSTextAlignment { get set }
```

## Discussion

The value of `mode` must be one of the alignments described in NSTextAlignment.

Text using `NSNaturalTextAlignment` is actually displayed using one of the other alignments, depending on the natural alignment of the text’s script.

## See Also

### Setting text alignment

func alignCenter(Any?)

This action method applies center alignment to selected paragraphs (or all text if the receiver is a plain text object).

func alignLeft(Any?)

This action method applies left alignment to selected paragraphs (or all text if the receiver is a plain text object).

func alignRight(Any?)

This action method applies right alignment to selected paragraphs (or all text if the receiver is a plain text object).

