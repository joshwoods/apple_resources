

- AppKit
- NSAppearanceCustomization
-  effectiveAppearance 

Instance Property

# effectiveAppearance

The appearance that will be used when the receiver is drawn onscreen, in an `NSAppearance` object. (read-only)

macOS 10.9+

``` source
var effectiveAppearance: NSAppearance { get }
```

**Required**

## Discussion

The default value for this property is provided by the nearest ancestor of the receiver that has set an appearance.

You can use this property to ensure that an offscreen view sets the appropriate current appearance when it draws onscreen.

## See Also

### Getting and Setting Appearance

Choosing a Specific Appearance for Your macOS App

Adopt a specific appearance for your windows, views, or app when it is inappropriate to support both light and dark variants.

var appearance: NSAppearance?

The appearance of the receiver, in an `NSAppearance` object.

**Required**

