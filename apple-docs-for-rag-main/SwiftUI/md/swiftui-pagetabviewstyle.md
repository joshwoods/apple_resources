

- SwiftUI
-  PageTabViewStyle 

Structure

# PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct PageTabViewStyle
```

## Overview

Use page or page(indexDisplayMode:) to construct this style.

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

## Topics

### Creating a page tab view style

init(indexDisplayMode: PageTabViewStyle.IndexDisplayMode)

Creates a new `PageTabViewStyle` with an index display mode

struct IndexDisplayMode

A style for displaying the page index view

## Relationships

### Conforms To

- TabViewStyle

## See Also

### Supporting types

struct DefaultTabViewStyle

The default tab view style.

struct SidebarAdaptableTabViewStyle

A tab bar style that adapts to each platform.

struct TabBarOnlyTabViewStyle

A tab view style that displays a tab bar when possible.

struct GroupedTabViewStyle

A tab view style that displays a tab bar that groups its tabs together.

struct VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical `TabView` interaction and appearance.

struct CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

