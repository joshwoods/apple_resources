

- SwiftUI
- TabViewStyle
-  carousel Deprecated

Type Property

# carousel

A style that implements the carousel interaction and appearance.

watchOS 7.0–11.4Deprecated

``` source
@MainActor @preconcurrency
static var carousel: CarouselTabViewStyle { get }
```

Available when `Self` is `CarouselTabViewStyle`.

Deprecated

Use verticalPage or verticalPage(transitionStyle:) instead.

## See Also

### Getting built-in tab view styles

static var automatic: DefaultTabViewStyle

The default tab view style.

static var page: PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

static func page(indexDisplayMode: PageTabViewStyle.IndexDisplayMode) -> PageTabViewStyle

A `TabViewStyle` that implements a paged scrolling `TabView` with an index display mode.

static var verticalPage: VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical page `TabView` interaction and appearance.

static func verticalPage(transitionStyle: VerticalPageTabViewStyle.TransitionStyle) -> VerticalPageTabViewStyle

A `TabViewStyle` that implements the vertical page `TabView` interaction and appearance, and performs the specified transition.

