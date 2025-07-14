

- UIKit
- NSTextLayoutManager
-  enumerateRenderingAttributes(from:reverse:using:) 

Instance Method

# enumerateRenderingAttributes(from:reverse:using:)

Enumerates the rendering attributes from a location you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func enumerateRenderingAttributes(
    from location: any NSTextLocation,
    reverse: Bool,
    using block: (NSTextLayoutManager, [NSAttributedString.Key : Any], NSTextRange) -> Bool
)
```

## Parameters 

`location`  

The location at which to start the enumeration.

`reverse`  

Whether to start the enumeration from the end of the range.

`block`  

A closure you provide to determine if the enumeration finishes early.

## Discussion

This method only enumerates ranges with text that specify rendering attributes. Returning `false` from `block` breaks out of the enumeration.

## See Also

### Adjusting rendering

class var linkRenderingAttributes: [NSAttributedString.Key : Any]

Returns the default set of attributes for rendering a link.

func addRenderingAttribute(NSAttributedString.Key, value: Any?, for: NSTextRange)

Sets the rendering attribute for the value and range you specify.

func renderingAttributes(forLink: Any, at: any NSTextLocation) -> [NSAttributedString.Key : Any]

Returns a dictionary of rendering attributes for rendering a link.

func invalidateRenderingAttributes(for: NSTextRange)

Invalidates the rendering attributes of the specified text range.

func removeRenderingAttribute(NSAttributedString.Key, for: NSTextRange)

Removes the rendering attribute from the specified text range.

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

