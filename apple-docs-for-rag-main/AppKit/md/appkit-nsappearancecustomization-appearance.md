

- AppKit
- NSAppearanceCustomization
-  appearance 

Instance Property

# appearance

The appearance of the receiver, in an `NSAppearance` object.

macOS 10.9+

``` source
var appearance: NSAppearance? { get set }
```

**Required**

## Mentioned in 

Choosing a Specific Appearance for Your macOS App

## Discussion

The default value for this property is `nil`, which means that the receiver uses the appearance it inherits from the nearest ancestor that has set an appearance. When you set `appearance` to a non-`nil` value, the receiver and the views it contains use the specified appearance.

## See Also

### Getting and Setting Appearance

Choosing a Specific Appearance for Your macOS App

Adopt a specific appearance for your windows, views, or app when it is inappropriate to support both light and dark variants.

var effectiveAppearance: NSAppearance

The appearance that will be used when the receiver is drawn onscreen, in an `NSAppearance` object. (read-only)

**Required**

