

- CarPlay
- CPDashboardButton
-  subtitleVariants 

Instance Property

# subtitleVariants

The array of subtitle variants for the button.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var subtitleVariants: [String] { get }
```

## Discussion

An array of subtitle variants for this button in an arrangement from most- to least-preferred. The system selects a subtitle from this array that best fits the available space. You provide the subtitle variants to init(titleVariants:subtitleVariants:image:handler:) as localized, displayable content.

## See Also

### Accessing the Button Configuration

var titleVariants: [String]

The array of title variants for the button.

var image: UIImage

The image the button displays.

