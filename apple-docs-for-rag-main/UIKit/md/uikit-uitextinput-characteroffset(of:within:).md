

- UIKit
- UITextInput
-  characterOffset(of:within:) 

Instance Method

# characterOffset(of:within:)

Returns the character offset of a position in a document’s text that falls within a specified range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func characterOffset(
    of position: UITextPosition,
    within range: UITextRange
) -> Int
```

## Parameters 

`position`  

An object that identifies a location in a document’s text.

`range`  

An object that specifies a range of text in a document.

## Return Value

The number of characters in a document’s text that occur between `position` and the beginning of `range`.

## Discussion

You should implement this method if you don’t have a one-to-one correspondence between UITextPosition objects within the given range and character offsets into a document string.

## See Also

### Reconciling text position and character offset

func position(within: UITextRange, atCharacterOffset: Int) -> UITextPosition?

Returns the position within a range of a document’s text that corresponds to the character offset from the start of that range.

