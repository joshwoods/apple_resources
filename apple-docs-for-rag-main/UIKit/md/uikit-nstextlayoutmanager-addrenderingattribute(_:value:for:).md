

- UIKit
- NSTextLayoutManager
-  addRenderingAttribute(\_:value:for:) 

Instance Method

# addRenderingAttribute(\_:value:for:)

Sets the rendering attribute for the value and range you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func addRenderingAttribute(
    _ renderingAttribute: NSAttributedString.Key,
    value: Any?,
    for textRange: NSTextRange
)
```

## Parameters 

`renderingAttribute`  

The NSAttributedString.Key that represents the attribute.

`value`  

The value for the attribute.

`textRange`  

The range over which to apply the attribute.

## Discussion

Passing `nil` overrides the specified attribute by removing it from the final attributes the framework passes to the layout and rendering engine. This is a convenience method for setRenderingAttributes(_:for:).

## See Also

### Adjusting rendering

class var linkRenderingAttributes: [NSAttributedString.Key : Any]

Returns the default set of attributes for rendering a link.

func enumerateRenderingAttributes(from: any NSTextLocation, reverse: Bool, using: (NSTextLayoutManager, [NSAttributedString.Key : Any], NSTextRange) -> Bool)

Enumerates the rendering attributes from a location you specify.

func renderingAttributes(forLink: Any, at: any NSTextLocation) -> [NSAttributedString.Key : Any]

Returns a dictionary of rendering attributes for rendering a link.

func invalidateRenderingAttributes(for: NSTextRange)

Invalidates the rendering attributes of the specified text range.

func removeRenderingAttribute(NSAttributedString.Key, for: NSTextRange)

Removes the rendering attribute from the specified text range.

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

