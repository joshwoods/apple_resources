

- UIKit
- UITextInput
-  setBaseWritingDirection(\_:for:) 

Instance Method

# setBaseWritingDirection(\_:for:)

Sets the base writing direction for a specified range of text in a document.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func setBaseWritingDirection(
    _ writingDirection: NSWritingDirection,
    for range: UITextRange
)
```

**Required**

## Parameters 

`writingDirection`  

A constant that represents a writing direction (for example, left-to-right or right-to-left)

`range`  

An object that represents a range of text in a document.

## See Also

### Determining layout and writing direction

func position(within: UITextRange, farthestIn: UITextLayoutDirection) -> UITextPosition?

Returns the text position that is at the farthest extent in a specified layout direction within a range of text.

**Required**

func characterRange(byExtending: UITextPosition, in: UITextLayoutDirection) -> UITextRange?

Returns a text range from a specified text position to its farthest extent in a certain direction of layout.

**Required**

func baseWritingDirection(for: UITextPosition, in: UITextStorageDirection) -> NSWritingDirection

Returns the base writing direction for a position in the text going in a certain direction.

**Required**

