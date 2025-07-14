

- UIKit
- UISearchTextField
-  tokenBackgroundColor 

Instance Property

# tokenBackgroundColor

The background color for all tokens in the search text field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var tokenBackgroundColor: UIColor! { get set }
```

## Discussion

If you set this property to `nil`, the search field reverts to the default token background color.

## See Also

### Customizing token behavior

func tokens(in: UITextRange) -> [UISearchToken]

Returns the search field’s tokens that are within a given range.

func positionOfToken(at: Int) -> UITextPosition

Converts a token index into a text position.

