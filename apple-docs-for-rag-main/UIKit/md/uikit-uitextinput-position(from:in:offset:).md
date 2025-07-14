

- UIKit
- UITextInput
-  position(from:in:offset:) 

Instance Method

# position(from:in:offset:)

Returns the text position at a specified offset in a specified direction from another text position.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func position(
    from position: UITextPosition,
    in direction: UITextLayoutDirection,
    offset: Int
) -> UITextPosition?
```

**Required**

## Parameters 

`position`  

A custom UITextPosition object that represents a location in a document.

`direction`  

A UITextLayoutDirection constant that represents the direction of the offset from `position`. Return `nil` if the computed text position is less than 0 or greater than the length of the backing string.

`offset`  

A character offset from `position`.

## Discussion

For an example of an implementation of the related method, position(from:offset:), see Using Text Kit to Draw and Manage Text in Text Programming Guide for iOS.

## See Also

### Computing text ranges and text positions

func textRange(from: UITextPosition, to: UITextPosition) -> UITextRange?

Returns the range between two text positions.

**Required**

func position(from: UITextPosition, offset: Int) -> UITextPosition?

Returns the text position at a specified offset from another text position.

**Required**

var beginningOfDocument: UITextPosition

The text position for the beginning of a document.

**Required**

var endOfDocument: UITextPosition

The text position for the end of a document.

**Required**

