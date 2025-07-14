

- AppKit
- NSTextLayoutManager
-  linkRenderingAttributes 

Type Property

# linkRenderingAttributes

Returns the default set of attributes for rendering a link.

macOS 12.0+

``` source
class var linkRenderingAttributes: [NSAttributedString.Key : Any] { get }
```

## Discussion

The base NSTextLayoutManager class returns with single for underlineStyle and the platform link color for foregroundColor. The platform color for macOS is `linkColor`. Other platforms uses `blueColor`.

## See Also

### Adjusting rendering

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

func setRenderingAttributes([NSAttributedString.Key : Any], for: NSTextRange)

Sets the rendering attributes for the range you specify.

