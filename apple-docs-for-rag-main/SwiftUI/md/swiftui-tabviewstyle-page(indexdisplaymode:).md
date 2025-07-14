

- SwiftUI
- TabViewStyle
-  page(indexDisplayMode:) 

Type Method

# page(indexDisplayMode:)

A `TabViewStyle` that implements a paged scrolling `TabView` with an index display mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
static func page(indexDisplayMode: PageTabViewStyle.IndexDisplayMode) -> PageTabViewStyle
```

Available when `Self` is `PageTabViewStyle`.

## Discussion

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

## See Also

### Getting built-in tab view styles

static var automatic: DefaultTabViewStyle

The default tab view style.

static var carousel: CarouselTabViewStyle

A style that implements the carousel interaction and appearance.

Deprecated

static var page: PageTabViewStyle

A `TabViewStyle` that displays a paged scrolling `TabView`.

static var verticalPage: VerticalPageTabViewStyle

A `TabViewStyle` that displays a vertical page `TabView` interaction and appearance.

static func verticalPage(transitionStyle: VerticalPageTabViewStyle.TransitionStyle) -> VerticalPageTabViewStyle

A `TabViewStyle` that implements the vertical page `TabView` interaction and appearance, and performs the specified transition.

