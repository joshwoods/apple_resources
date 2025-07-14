

- SwiftUI
-  VerticalPageTabViewStyle 

Structure

# VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical `TabView` interaction and appearance.

watchOS 10.0+

``` source
struct VerticalPageTabViewStyle
```

## Overview

Use verticalPage to construct this style.

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

## Topics

### Creating the tab view style

init()

init(transitionStyle: VerticalPageTabViewStyle.TransitionStyle)

Creates a new `VerticalPageTabViewStyle` with a transition style.

struct TransitionStyle

A transition style used between tabs.

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

struct PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

struct CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

