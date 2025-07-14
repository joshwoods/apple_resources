

- UIKit
- UITextInput
-  insertTextPlaceholder(with:) 

Instance Method

# insertTextPlaceholder(with:)

Inserts a placeholder object to reserve visual space during text input.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func insertTextPlaceholder(with size: CGSize) -> UITextPlaceholder
```

## Parameters 

`size`  

The size of the space to reserve.

## Return Value

The placeholder object that was inserted into the text input.

## Discussion

If the `size.height` is less than or equal to zero, then the placeholder displays inline using the current line’s height.

If the `size.height` is greater than zero, then the text input treats the placeholder as a paragraph of height `size.height`.

## See Also

### Managing placeholders

func remove(UITextPlaceholder)

Removes a placeholder object from the text input view.

class UITextPlaceholder

A placeholder object that reserves visual space in a text input view.

