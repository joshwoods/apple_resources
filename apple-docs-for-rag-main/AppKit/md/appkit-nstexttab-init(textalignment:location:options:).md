

- AppKit
- NSTextTab
-  init(textAlignment:location:options:) 

Initializer

# init(textAlignment:location:options:)

Initializes a text tab with the specified text alignment, location, and options.

macOS 10.0+

``` source
init(
    textAlignment alignment: NSTextAlignment,
    location loc: CGFloat,
    options: [NSTextTab.OptionKey : Any] = [:]
)
```

## Parameters 

`alignment`  

The alignment of the text.

`loc`  

The position of the text tab on the ruler, relative to the back margin.

`options`  

Options to apply to the text tab.

## Return Value

An initialized text tab.

## Discussion

The text alignment is used to determine the position of text inside the tab column. See NSParagraphStyle.TextTabType for a mapping between alignments and tab stop types

