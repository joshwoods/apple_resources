

- AppKit
- NSTextLayoutFragment
-  init(textElement:range:) 

Initializer

# init(textElement:range:)

Create a new layout fragment using the provided text element and range.

macOS 12.0+

``` source
init(
    textElement: NSTextElement,
    range rangeInElement: NSTextRange?
)
```

## Parameters 

`textElement`  

An NSTextElement.

`rangeInElement`  

A range that defines the boundaries of the text for the new layout fragment.

## See Also

### Creating a layout fragment

init?(coder: NSCoder)

Creates a new layout fragment with the coder you provide.

