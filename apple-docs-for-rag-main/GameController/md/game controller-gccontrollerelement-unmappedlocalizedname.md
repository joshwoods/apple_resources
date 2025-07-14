

- Game Controller
- GCControllerElement
-  unmappedLocalizedName 

Instance Property

# unmappedLocalizedName

The element’s localized name, not the remapped name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var unmappedLocalizedName: String? { get set }
```

## Discussion

To present the element that a user wants to remap in your interface, use this property to get the original name. Otherwise, use the localizedName property to get the possibly remapped name.

## See Also

### Getting a localized name

var localizedName: String?

The localized name for the element or the remapped element.

