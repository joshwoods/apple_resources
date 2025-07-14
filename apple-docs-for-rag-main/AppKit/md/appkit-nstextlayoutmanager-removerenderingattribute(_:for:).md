

- AppKit
- NSTextLayoutManager
-  removeRenderingAttribute(\_:for:) 

Instance Method

# removeRenderingAttribute(\_:for:)

Removes the rendering attribute from the specified text range.

macOS 12.0+

``` source
func removeRenderingAttribute(
    _ renderingAttribute: NSAttributedString.Key,
    for textRange: NSTextRange
)
```

## Parameters 

`renderingAttribute`  

The NSAttributedString.Key attribute to remove

`textRange`  

The range over which to remove the rendering attribute.

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

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

