

- SwiftUI
-  ListStyle 

Protocol

# ListStyle

A protocol that describes the behavior and appearance of a list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ListStyle
```

## Topics

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

static var sidebar: SidebarListStyle

The list style that describes the behavior and appearance of a sidebar list.

### Deprecated styles

static func bordered(alternatesRowBackgrounds: Bool) -> BorderedListStyle

The list style that describes the behavior and appearance of a list with standard border.

Deprecated

static func inset(alternatesRowBackgrounds: Bool) -> InsetListStyle

The list style that describes the behavior and appearance of an inset list with optional alternating row backgrounds.

Deprecated

### Supporting types

struct DefaultListStyle

The list style that describes a platform’s default behavior and appearance for a list.

struct BorderedListStyle

The list style that describes the behavior and appearance of a list with standard border.

struct CarouselListStyle

The carousel list style.

struct EllipticalListStyle

The list style that describes the behavior and appearance of an elliptical list.

struct GroupedListStyle

The list style that describes the behavior and appearance of a grouped list.

struct InsetListStyle

The list style that describes the behavior and appearance of an inset list.

struct InsetGroupedListStyle

The list style that describes the behavior and appearance of an inset grouped list.

struct PlainListStyle

The list style that describes the behavior and appearance of a plain list.

struct SidebarListStyle

The list style that describes the behavior and appearance of a sidebar list.

## Relationships

### Conforming Types

- BorderedListStyle
- CarouselListStyle
- DefaultListStyle
- EllipticalListStyle
- GroupedListStyle
- InsetGroupedListStyle
- InsetListStyle
- PlainListStyle
- SidebarListStyle

## See Also

### Styling collection views

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

func tableStyle&lt;S>(S) -> some View

Sets the style for tables within this view.

protocol TableStyle

A type that applies a custom appearance to all tables within a view.

struct TableStyleConfiguration

The properties of a table.

func disclosureGroupStyle&lt;S>(S) -> some View

Sets the style for disclosure groups within this view.

protocol DisclosureGroupStyle

A type that specifies the appearance and interaction of disclosure groups within a view hierarchy.

