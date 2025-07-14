

- UIKit
- UITextInput
-  position(within:atCharacterOffset:) 

Instance Method

# position(within:atCharacterOffset:)

Returns the position within a range of a document’s text that corresponds to the character offset from the start of that range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func position(
    within range: UITextRange,
    atCharacterOffset offset: Int
) -> UITextPosition?
```

## Parameters 

`range`  

An object that specifies a range of text in a document.

`offset`  

A character offset from the start of `range`.

## Return Value

An object that represents a position in a document’s visible text.

## Discussion

You should implement this method if you don’t have a one-to-one correspondence between UITextPosition objects within the given range and character offsets into a document string.

## See Also

### Reconciling text position and character offset

func characterOffset(of: UITextPosition, within: UITextRange) -> Int

Returns the character offset of a position in a document’s text that falls within a specified range.

