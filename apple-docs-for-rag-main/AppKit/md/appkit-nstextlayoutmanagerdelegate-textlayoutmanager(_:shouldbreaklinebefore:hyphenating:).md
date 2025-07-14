

- AppKit
- NSTextLayoutManagerDelegate
-  textLayoutManager(\_:shouldBreakLineBefore:hyphenating:) 

Instance Method

# textLayoutManager(\_:shouldBreakLineBefore:hyphenating:)

The method the framework calls to determine the soft line break point.

macOS 12.0+

``` source
optional func textLayoutManager(
    _ textLayoutManager: NSTextLayoutManager,
    shouldBreakLineBefore location: any NSTextLocation,
    hyphenating: Bool
) -> Bool
```

## Parameters 

`textLayoutManager`  

The text layout manager.

`location`  

The location of the proposed line break.

`hyphenating`  

A Boolean value that indicates the current hyphenation mode.

## Return Value

A Boolean value that indicates if the framework should break the line at the current location.

## Discussion

When `hyphenating` is `false`, `NSTextLayoutManager` tries to find the next line break opportunity before location. When hyphenating is `true`, it’s an auto-hyphenation point.

## See Also

### Responding to layout changes

func textLayoutManager(NSTextLayoutManager, renderingAttributesForLink: Any, at: any NSTextLocation, defaultAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]?

The method the framework calls to return a dictionary of attributes for rendering a link attribute name.

func textLayoutManager(NSTextLayoutManager, textLayoutFragmentFor: any NSTextLocation, in: NSTextElement) -> NSTextLayoutFragment

The method the framework calls to give the delegate an opportunity to return a custom text layout fragment.

