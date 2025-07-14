

- UIKit
- UITextInput
-  position(from:offset:) 

Instance Method

# position(from:offset:)

Returns the text position at a specified offset from another text position.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func position(
    from position: UITextPosition,
    offset: Int
) -> UITextPosition?
```

**Required**

## Parameters 

`position`  

A custom UITextPosition object that represents a location in a document.

`offset`  

A character offset from `position`. It can be a positive or negative value.

## Return Value

A custom UITextPosition object that represents the location in a document that is at the specified offset from `position`. Return `nil` if the computed text position is less than 0 or greater than the length of the backing string.

## Discussion

For an example of an implementation of this method, see Using Text Kit to Draw and Manage Text in Text Programming Guide for iOS.

## See Also

### Computing text ranges and text positions

func textRange(from: UITextPosition, to: UITextPosition) -> UITextRange?

Returns the range between two text positions.

**Required**

func position(from: UITextPosition, in: UITextLayoutDirection, offset: Int) -> UITextPosition?

Returns the text position at a specified offset in a specified direction from another text position.

**Required**

var beginningOfDocument: UITextPosition

The text position for the beginning of a document.

**Required**

var endOfDocument: UITextPosition

The text position for the end of a document.

**Required**

