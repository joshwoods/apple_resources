

- AppKit
- NSTextLayoutManagerDelegate
-  textLayoutManager(\_:renderingAttributesForLink:at:defaultAttributes:) 

Instance Method

# textLayoutManager(\_:renderingAttributesForLink:at:defaultAttributes:)

The method the framework calls to return a dictionary of attributes for rendering a link attribute name.

macOS 12.0+

``` source
optional func textLayoutManager(
    _ textLayoutManager: NSTextLayoutManager,
    renderingAttributesForLink link: Any,
    at location: any NSTextLocation,
    defaultAttributes renderingAttributes: [NSAttributedString.Key : Any] = [:]
) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`textLayoutManager`  

The `NSTextLayoutManager`.

`link`  

The link.

`location`  

The NSTextLocation of the link.

`renderingAttributes`  

A dictionary of attributes whose keys are NSAttributedString.Key values.

## Return Value

A dictionary of attributes.

## See Also

### Responding to layout changes

func textLayoutManager(NSTextLayoutManager, shouldBreakLineBefore: any NSTextLocation, hyphenating: Bool) -> Bool

The method the framework calls to determine the soft line break point.

func textLayoutManager(NSTextLayoutManager, textLayoutFragmentFor: any NSTextLocation, in: NSTextElement) -> NSTextLayoutFragment

The method the framework calls to give the delegate an opportunity to return a custom text layout fragment.

