

- UIKit
- UITextInput
-  baseWritingDirection(for:in:) 

Instance Method

# baseWritingDirection(for:in:)

Returns the base writing direction for a position in the text going in a certain direction.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func baseWritingDirection(
    for position: UITextPosition,
    in direction: UITextStorageDirection
) -> NSWritingDirection
```

**Required**

## Parameters 

`position`  

An object that identifies a location in a document.

`direction`  

A constant that indicates a direction of storage (forward or backward).

## Return Value

A constant that represents a writing direction (for example, left-to-right or right-to-left).

## Discussion

The base writing direction is set previously when the text input system sends a setBaseWritingDirection(_:for:) message to the conforming document object.

## See Also

### Determining layout and writing direction

func position(within: UITextRange, farthestIn: UITextLayoutDirection) -> UITextPosition?

Returns the text position that is at the farthest extent in a specified layout direction within a range of text.

**Required**

func characterRange(byExtending: UITextPosition, in: UITextLayoutDirection) -> UITextRange?

Returns a text range from a specified text position to its farthest extent in a certain direction of layout.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

