

- UIKit
- UITextPasteItem
-  setResult(string:) 

Instance Method

# setResult(string:)

Sets a text paste item’s textual value to a specified plaintext string from the item provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setResult(string: String)
```

**Required**

## See Also

### Setting a text paste item’s result value

func setResult(attributedString: NSAttributedString)

Sets a text paste item’s textual value to a specified attributed string from the item provider.

**Required**

func setResult(attachment: NSTextAttachment)

Sets a text paste item’s attachment value to a specified value.

**Required**

func setDefaultResult()

Sets the text paste item’s value to the default value based on the item provider’s data.

**Required**

func setNoResult()

Sets the text paste item’s textual value to not include data from the item provider.

**Required**

