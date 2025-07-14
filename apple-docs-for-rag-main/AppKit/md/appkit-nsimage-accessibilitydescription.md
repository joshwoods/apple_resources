

- AppKit
- NSImage
-  accessibilityDescription 

Instance Property

# accessibilityDescription

The image’s accessibility description.

macOS 10.6+

``` source
var accessibilityDescription: String? { get set }
```

## Discussion

This description is used automatically by interface elements that display images. Like all accessibility descriptions, use a short localized string that does not include the name of the interface element. For instance, “delete” rather than “delete button”.

