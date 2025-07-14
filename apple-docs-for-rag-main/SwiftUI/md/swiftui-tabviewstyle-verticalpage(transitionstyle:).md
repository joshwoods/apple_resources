

- SwiftUI
- TabViewStyle
-  verticalPage(transitionStyle:) 

Type Method

# verticalPage(transitionStyle:)

A `TabViewStyle` that implements the vertical page `TabView` interaction and appearance, and performs the specified transition.

watchOS 10.0+

``` source
@MainActor @preconcurrency
static func verticalPage(transitionStyle: VerticalPageTabViewStyle.TransitionStyle) -> VerticalPageTabViewStyle
```

Available when `Self` is `VerticalPageTabViewStyle`.

## See Also

### Getting built-in tab view styles

static var automatic: DefaultTabViewStyle

The default tab view style.

static var carousel: CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

static var page: PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

static func page(indexDisplayMode: PageTabViewStyle.IndexDisplayMode) -> PageTabViewStyle

A `TabViewStyle` that implements a paged scrolling `TabView` with an index display mode.

static var verticalPage: VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical page `TabView` interaction and appearance.

