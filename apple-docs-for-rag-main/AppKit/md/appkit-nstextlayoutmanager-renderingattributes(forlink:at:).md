

- AppKit
- NSTextLayoutManager
-  renderingAttributes(forLink:at:) 

Instance Method

# renderingAttributes(forLink:at:)

Returns a dictionary of rendering attributes for rendering a link.

macOS 12.0+

``` source
func renderingAttributes(
    forLink link: Any,
    at location: any NSTextLocation
) -> [NSAttributedString.Key : Any]
```

## Parameters 

`link`  

The link.

`location`  

The location of the link in the text.

## Return Value

A dictionary of rendering attributes.

## Discussion

As with other rendering attributes, specifying NSNull removes the attribute from the final attributes the framework uses for rendering. It has priority over the general rendering attributes.

## See Also

### Adjusting rendering

class var linkRenderingAttributes: [NSAttributedString.Key : Any]

Returns the default set of attributes for rendering a link.

func addRenderingAttribute(NSAttributedString.Key, value: Any?, for: NSTextRange)

Sets the rendering attribute for the value and range you specify.

func enumerateRenderingAttributes(from: any NSTextLocation, reverse: Bool, using: (NSTextLayoutManager, [NSAttributedString.Key : Any], NSTextRange) -> Bool)

Enumerates the rendering attributes from a location you specify.

func invalidateRenderingAttributes(for: NSTextRange)

Invalidates the rendering attributes of the specified text range.

func removeRenderingAttribute(NSAttributedString.Key, for: NSTextRange)

Removes the rendering attribute from the specified text range.

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

