

- UIKit
- NSTextLayoutManager
-  setRenderingAttributes(\_:for:) 

Instance Method

# setRenderingAttributes(\_:for:)

Sets the rendering attributes for the range you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func setRenderingAttributes(
    _ renderingAttributes: [NSAttributedString.Key : Any],
    for textRange: NSTextRange
)
```

## Parameters 

`renderingAttributes`  

A dictionary of rendering attributes.

`textRange`  

The text range over which to apply `renderingAttributes`.

## See Also

### Adjusting rendering

class var linkRenderingAttributes: [NSAttributedString.Key : Any]

Returns the default set of attributes for rendering a link.

func addRenderingAttribute(NSAttributedString.Key, value: Any?, for: NSTextRange)

Sets the rendering attribute for the value and range you specify.

func enumerateRenderingAttributes(from: any NSTextLocation, reverse: Bool, using: (NSTextLayoutManager, [NSAttributedString.Key : Any], NSTextRange) -> Bool)

Enumerates the rendering attributes from a location you specify.

func renderingAttributes(forLink: Any, at: any NSTextLocation) -> [NSAttributedString.Key : Any]

Returns a dictionary of rendering attributes for rendering a link.

func invalidateRenderingAttributes(for: NSTextRange)

Invalidates the rendering attributes of the specified text range.

func removeRenderingAttribute(NSAttributedString.Key, for: NSTextRange)

Removes the rendering attribute from the specified text range.

