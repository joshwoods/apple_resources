

- SwiftUI
- ListStyle
-  bordered 

Type Property

# bordered

The list style that describes the behavior and appearance of a list with standard border.

macOS 12.0+

``` source
static var bordered: BorderedListStyle { get }
```

Available when `Self` is `BorderedListStyle`.

## Discussion

Bordered lists are expected to be inset from their outer containers, but do not have inset style rows or selection.

To customize whether the rows of the list should alternate their backgrounds, use bordered(alternatesRowBackgrounds:).

## See Also

### Getting built-in list styles

static var automatic: DefaultListStyle

The list style that describes a platform’s default behavior and appearance for a list.

static var carousel: CarouselListStyle

The carousel list style.

static var elliptical: EllipticalListStyle

The list style that describes the behavior and appearance of an elliptical list.

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

