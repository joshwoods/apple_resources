

- UIKit
- UIGraphicsImageRendererFormat
-  prefersExtendedRange Deprecated

Instance Property

# prefersExtendedRange

A Boolean value that specifies whether the bitmap context uses extended color.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–12.0Deprecated

``` source
var prefersExtendedRange: Bool { get set }
```

Deprecated

Use preferredRange instead.

## Discussion

If true, the underlying Core Graphics context is configured to support wide color; if false, the context is not.

The default is true on devices that natively support wide color, and false on those that do not.

## See Also

### Configuring the renderer attributes

var opaque: Bool

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

var scale: CGFloat

The display scale of the image renderer context.

var preferredRange: UIGraphicsImageRendererFormat.Range

The preferred color range of the image renderer context.

enum Range

Constants that specify the color range of the image renderer context.

