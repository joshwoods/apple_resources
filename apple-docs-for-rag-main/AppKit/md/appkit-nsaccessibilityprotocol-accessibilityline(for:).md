

- AppKit
- NSAccessibilityProtocol
-  accessibilityLine(for:) 

Instance Method

# accessibilityLine(for:)

Returns the line number for the line that contains the specified character index.

macOS 10.10+

``` source
func accessibilityLine(for index: Int) -> Int
```

**Required**

## Parameters 

`index`  

The index for a character.

## Return Value

The line number for the line holding the specified character index.

## See Also

### Configuring Text Elements

func accessibilityInsertionPointLineNumber() -> Int

Returns the line number that contains the insertion point.

**Required**

func setAccessibilityInsertionPointLineNumber(Int)

Sets the line number that contains the insertion point.

**Required**

func accessibilityNumberOfCharacters() -> Int

Returns the number of characters in the text.

**Required**

func setAccessibilityNumberOfCharacters(Int)

Sets the number of characters in the text.

**Required**

func accessibilityPlaceholderValue() -> String?

Returns the placeholder value for the accessibility element.

**Required**

func setAccessibilityPlaceholderValue(String?)

Sets the placeholder value for the accessibility element.

**Required**

func accessibilitySelectedText() -> String?

Returns the currently selected text.

**Required**

func setAccessibilitySelectedText(String?)

Sets the currently selected text.

**Required**

func accessibilitySelectedTextRange() -> NSRange

Returns the range of the currently selected text.

**Required**

func setAccessibilitySelectedTextRange(NSRange)

Sets the range of the currently selected text.

**Required**

func accessibilitySelectedTextRanges() -> [NSValue]?

Returns an array of ranges for the currently selected text.

**Required**

func setAccessibilitySelectedTextRanges([NSValue]?)

Sets an array of ranges for the currently selected text.

**Required**

func accessibilitySharedCharacterRange() -> NSRange

Returns the range of characters that the accessibility element displays.

**Required**

func setAccessibilitySharedCharacterRange(NSRange)

Sets the range of characters that the accessibility element displays.

**Required**

func accessibilitySharedTextUIElements() -> [Any]?

Returns the other elements that share text with the accessibility element.

**Required**

