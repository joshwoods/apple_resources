

- UIKit
- UITextInput
-  position(within:farthestIn:) 

Instance Method

# position(within:farthestIn:)

Returns the text position that is at the farthest extent in a specified layout direction within a range of text.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func position(
    within range: UITextRange,
    farthestIn direction: UITextLayoutDirection
) -> UITextPosition?
```

**Required**

## Parameters 

`range`  

A text-range object that demarcates a range of text in a document.

`direction`  

A constant that indicates a direction of layout (right, left, up, down).

## Return Value

A text-position object that identifies a location in the visible text.

## See Also

### Determining layout and writing direction

func characterRange(byExtending: UITextPosition, in: UITextLayoutDirection) -> UITextRange?

Returns a text range from a specified text position to its farthest extent in a certain direction of layout.

**Required**

func baseWritingDirection(for: UITextPosition, in: UITextStorageDirection) -> NSWritingDirection

Returns the base writing direction for a position in the text going in a certain direction.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

