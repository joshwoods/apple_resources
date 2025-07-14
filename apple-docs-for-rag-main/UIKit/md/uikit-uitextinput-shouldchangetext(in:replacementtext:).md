

- UIKit
- UITextInput
-  shouldChangeText(in:replacementText:) 

Instance Method

# shouldChangeText(in:replacementText:)

Asks whether to replace the text in the specified range.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func shouldChangeText(
    in range: UITextRange,
    replacementText text: String
) -> Bool
```

## Parameters 

`range`  

A range of text in a document.

`text`  

The proposed text to replace the text in `range`.

## Return Value

true if the text should be changed or false if it should not.

## Discussion

Prior to replacing text, this method is called to give your delegate a chance to accept or reject the edits. If you do not implement this method, the return value defaults to true.

## See Also

### Replacing and returning text

func text(in: UITextRange) -> String?

Returns the text in the specified range.

**Required**

func replace(UITextRange, withText: String)

Replaces the text in a document that is in the specified range.

**Required**

