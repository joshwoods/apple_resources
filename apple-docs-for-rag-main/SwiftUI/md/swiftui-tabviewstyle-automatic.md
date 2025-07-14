

- SwiftUI
- TabViewStyle
-  automatic 

Type Property

# automatic

The default tab view style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
static var automatic: DefaultTabViewStyle { get }
```

Available when `Self` is `DefaultTabViewStyle`.

## See Also

### Getting built-in tab view styles

static var carousel: CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

static var page: PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

static func page(indexDisplayMode: PageTabViewStyle.IndexDisplayMode) -> PageTabViewStyle

A `TabViewStyle` that implements a paged scrolling `TabView` with an index display mode.

static var verticalPage: VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical page `TabView` interaction and appearance.

static func verticalPage(transitionStyle: VerticalPageTabViewStyle.TransitionStyle) -> VerticalPageTabViewStyle

A `TabViewStyle` that implements the vertical page `TabView` interaction and appearance, and performs the specified transition.

