

- UIKit
- UITextPasteItem
-  setDefaultResult() 

Instance Method

# setDefaultResult()

Sets the text paste item’s value to the default value based on the item provider’s data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setDefaultResult()
```

**Required**

## Discussion

You call this method, as a fallback, for any items you don’t handle. Setting the default result when the item provider’s data isn’t supported is the same as calling the setNoResult() method.

## See Also

### Setting a text paste item’s result value

func setResult(string: String)

Sets a text paste item’s textual value to a specified plaintext string from the item provider.

**Required**

func setResult(attributedString: NSAttributedString)

Sets a text paste item’s textual value to a specified attributed string from the item provider.

**Required**

func setResult(attachment: NSTextAttachment)

Sets a text paste item’s attachment value to a specified value.

**Required**

func setNoResult()

Sets the text paste item’s textual value to not include data from the item provider.

**Required**

