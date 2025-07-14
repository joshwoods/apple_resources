

- SwiftUI
- ListStyle
-  elliptical 

Type Property

# elliptical

The list style that describes the behavior and appearance of an elliptical list.

watchOS 7.0+

``` source
static var elliptical: EllipticalListStyle { get }
```

Available when `Self` is `EllipticalListStyle`.

## Discussion

On watchOS, the elliptical list style uses a transform for items rolling off the top or bottom of the list, as if on a rounded surface that faces the user.

Apple Watch Series 3 does not support this style and will instead fall back to using the plain style.

## See Also

### Getting built-in list styles

static var automatic: DefaultListStyle

The list style that describes a platform’s default behavior and appearance for a list.

static var bordered: BorderedListStyle

The list style that describes the behavior and appearance of a list with standard border.

static var carousel: CarouselListStyle

The carousel list style.

static var grouped: GroupedListStyle

The list style that describes the behavior and appearance of a grouped list.

static var inset: InsetListStyle

The list style that describes the behavior and appearance of an inset list.

static var insetGrouped: InsetGroupedListStyle

The list style that describes the behavior and appearance of an inset grouped list.

static var plain: PlainListStyle

The list style that describes the behavior and appearance of a plain list.

static var sidebar: SidebarListStyle

The list style that describes the behavior and appearance of a sidebar list.

