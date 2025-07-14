

- UIKit
- UITextInput
-  textRange(from:to:) 

Instance Method

# textRange(from:to:)

Returns the range between two text positions.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func textRange(
    from fromPosition: UITextPosition,
    to toPosition: UITextPosition
) -> UITextRange?
```

**Required**

## Parameters 

`fromPosition`  

An object that represents a location in a document.

`toPosition`  

An object that represents another location in a document.

## Return Value

An object that represents the range between `fromPosition` and `toPosition`.

## See Also

### Computing text ranges and text positions

func position(from: UITextPosition, offset: Int) -> UITextPosition?

Returns the text position at a specified offset from another text position.

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

