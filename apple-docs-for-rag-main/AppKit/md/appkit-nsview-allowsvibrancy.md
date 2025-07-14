

- AppKit
- NSView
-  allowsVibrancy 

Instance Property

# allowsVibrancy

A Boolean value indicating whether the view ensures it is vibrant on top of other content.

macOS 10.10+

``` source
@MainActor
var allowsVibrancy: Bool { get }
```

## Discussion

AppKit checks this property when the view is incorporated into a view hierarchy that uses vibrancy. If the property is true, the view takes appropriate measures to ensure its content is vibrant on top of any underlying material. The default value of this property is false. However, some of AppKit’s view subclasses change the value of this property based on the artwork they draw.

