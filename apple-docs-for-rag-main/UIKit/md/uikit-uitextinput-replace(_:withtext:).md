

- UIKit
- UITextInput
-  replace(\_:withText:) 

Instance Method

# replace(\_:withText:)

Replaces the text in a document that is in the specified range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func replace(
    _ range: UITextRange,
    withText text: String
)
```

**Required**

## Parameters 

`range`  

A range of text in a document.

`text`  

A string to replace the text in `range`.

## See Also

### Replacing and returning text

func text(in: UITextRange) -> String?

Returns the text in the specified range.

**Required**

func shouldChangeText(in: UITextRange, replacementText: String) -> Bool

Asks whether to replace the text in the specified range.

