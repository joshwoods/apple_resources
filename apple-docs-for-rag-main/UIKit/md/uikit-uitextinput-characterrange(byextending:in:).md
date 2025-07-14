

- UIKit
- UITextInput
-  characterRange(byExtending:in:) 

Instance Method

# characterRange(byExtending:in:)

Returns a text range from a specified text position to its farthest extent in a certain direction of layout.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func characterRange(
    byExtending position: UITextPosition,
    in direction: UITextLayoutDirection
) -> UITextRange?
```

**Required**

## Parameters 

`position`  

A text-position object that identifies a location in a document.

`direction`  

A constant that indicates a direction of layout (right, left, up, down).

## Return Value

A text-range object that represents the distance from `position` to the farthest extent in `direction`.

## See Also

### Determining layout and writing direction

func position(within: UITextRange, farthestIn: UITextLayoutDirection) -> UITextPosition?

Returns the text position that is at the farthest extent in a specified layout direction within a range of text.

**Required**

func baseWritingDirection(for: UITextPosition, in: UITextStorageDirection) -> NSWritingDirection

Returns the base writing direction for a position in the text going in a certain direction.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

