

- AppKit
- NSAnimationContext
-  allowsImplicitAnimation 

Instance Property

# allowsImplicitAnimation

Determine if animations are enabled or not for animations that occur as a result of another property change.

macOS 10.8+

``` source
var allowsImplicitAnimation: Bool { get set }
```

## Discussion

Using the animator() proxy will automatically set `allowsImplicitAnimation` to true. When true, other properties can implicitly animate along with the initially changed property.

For instance, calling `[[view animator] setFrame:frame]` will allow subviews to also animate their frame positions. When the value is false the behavior is diabled.

The default value is false.

This is only applicable when layer backed on OS v10.8 and later.

