

- SwiftUI
- ListStyle
-  insetGrouped 

Type Property

# insetGrouped

The list style that describes the behavior and appearance of an inset grouped list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
static var insetGrouped: InsetGroupedListStyle { get }
```

Available when `Self` is `InsetGroupedListStyle`.

## Discussion

On iOS, the inset grouped list style displays a continuous background color that extends from the section header, around both sides of list items in the section, and down to the section footer. This visually groups the items to a greater degree than either the inset or grouped styles do.

## See Also

### Getting built-in list styles

static var automatic: DefaultListStyle

The list style that describes a platform’s default behavior and appearance for a list.

static var bordered: BorderedListStyle

The list style that describes the behavior and appearance of a list with standard border.

static var carousel: CarouselListStyle

The carousel list style.

static var elliptical: EllipticalListStyle

The list style that describes the behavior and appearance of an elliptical list.

static var grouped: GroupedListStyle

The list style that describes the behavior and appearance of a grouped list.

static var inset: InsetListStyle

The list style that describes the behavior and appearance of an inset list.

static var plain: PlainListStyle

The list style that describes the behavior and appearance of a plain list.

static var sidebar: SidebarListStyle

The list style that describes the behavior and appearance of a sidebar list.

