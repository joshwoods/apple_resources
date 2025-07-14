

- UIKit
- UITextInput
-  text(in:) 

Instance Method

# text(in:)

Returns the text in the specified range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func text(in range: UITextRange) -> String?
```

**Required**

## Parameters 

`range`  

A range of text in a document.

## Return Value

A substring of a document that falls within the specified range.

## See Also

### Replacing and returning text

func replace(UITextRange, withText: String)

Replaces the text in a document that is in the specified range.

**Required**

func shouldChangeText(in: UITextRange, replacementText: String) -> Bool

Asks whether to replace the text in the specified range.

