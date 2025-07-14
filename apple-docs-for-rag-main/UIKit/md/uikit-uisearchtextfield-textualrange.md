

- UIKit
- UISearchTextField
-  textualRange 

Instance Property

# textualRange

The range of the field’s text content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var textualRange: UITextRange { get }
```

## Discussion

Both tokens and text are included in the range from beginningOfDocument to endOfDocument. This property provides convenient access to just the text.

## See Also

### Converting text into tokens

func replaceTextualPortion(of: UITextRange, with: UISearchToken, at: Int)

Converts text in a search field into a search token.

