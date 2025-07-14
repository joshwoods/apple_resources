

- SwiftUI
- ListStyle
-  sidebar 

Type Property

# sidebar

The list style that describes the behavior and appearance of a sidebar list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
static var sidebar: SidebarListStyle { get }
```

Available when `Self` is `SidebarListStyle`.

## Discussion

On macOS and iOS, the sidebar list style displays disclosure indicators in the section headers that allow the user to collapse and expand sections.

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

static var insetGrouped: InsetGroupedListStyle

The list style that describes the behavior and appearance of an inset grouped list.

static var plain: PlainListStyle

The list style that describes the behavior and appearance of a plain list.

