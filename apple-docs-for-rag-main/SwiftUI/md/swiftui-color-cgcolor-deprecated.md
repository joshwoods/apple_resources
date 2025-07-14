

- SwiftUI
- Color
-  cgColor Deprecated

Instance Property

# cgColor

A Core Graphics representation of the color, if available.

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0–18.4DeprecatedmacOS 11.0–15.4DeprecatedtvOS 14.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 7.0–11.4Deprecated

``` source
var cgColor: CGColor? { get }
```

## Discussion

You can get a CGColor instance from a constant SwiftUI color. This includes colors you create from a Core Graphics color, from RGB or HSB components, or from constant UIKit and AppKit colors.

For a dynamic color, like one you load from an Asset Catalog using init(_:bundle:), or one you create from a dynamic UIKit or AppKit color, this property is `nil`. To evaluate all types of colors, use the `resolve(in:)` method.

