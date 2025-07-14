

- UIKit
- UITabBarAppearance
-  inlineLayoutAppearance 

Instance Property

# inlineLayoutAppearance

The appearance attributes for items displayed with an inline style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var inlineLayoutAppearance: UITabBarItemAppearance { get set }
```

## Discussion

If you didn’t provide a set of explicit attributes at initialization time, UIKit provides an object with default attributes.

## See Also

### Configuring inline item appearances

var compactInlineLayoutAppearance: UITabBarItemAppearance

The appearance attributes for items displayed with an inline style in a compact environment.

