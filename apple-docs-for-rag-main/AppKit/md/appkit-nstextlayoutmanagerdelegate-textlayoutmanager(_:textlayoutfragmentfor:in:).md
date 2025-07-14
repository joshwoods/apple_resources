

- AppKit
- NSTextLayoutManagerDelegate
-  textLayoutManager(\_:textLayoutFragmentFor:in:) 

Instance Method

# textLayoutManager(\_:textLayoutFragmentFor:in:)

The method the framework calls to give the delegate an opportunity to return a custom text layout fragment.

macOS 12.0+

``` source
optional func textLayoutManager(
    _ textLayoutManager: NSTextLayoutManager,
    textLayoutFragmentFor location: any NSTextLocation,
    in textElement: NSTextElement
) -> NSTextLayoutFragment
```

## Parameters 

`textLayoutManager`  

The text layout manager.

`location`  

The NSTextLocation of the link in the text element.

`textElement`  

The NSTextElement that the method could return a custom NSTextLayoutFragment from.

## Return Value

An NSTextLayoutFragment.

## Discussion

Use this to provide an NSTextLayoutFragment specialized for an NSTextElement subclass targeted for the rendering surface.

## See Also

### Responding to layout changes

func textLayoutManager(NSTextLayoutManager, renderingAttributesForLink: Any, at: any NSTextLocation, defaultAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]?

The method the framework calls to return a dictionary of attributes for rendering a link attribute name.

func textLayoutManager(NSTextLayoutManager, shouldBreakLineBefore: any NSTextLocation, hyphenating: Bool) -> Bool

The method the framework calls to determine the soft line break point.

