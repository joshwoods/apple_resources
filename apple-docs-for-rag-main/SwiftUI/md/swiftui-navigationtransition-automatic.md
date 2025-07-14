

- SwiftUI
- NavigationTransition
-  automatic 

Type Property

# automatic

A style that automatically chooses the appropriate presentation transition for the current context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var automatic: AutomaticNavigationTransition { get }
```

Available when `Self` is `AutomaticNavigationTransition`.

## See Also

### Getting built-in transitions

static func zoom(sourceID: some Hashable, in: Namespace.ID) -> ZoomNavigationTransition

A navigation transition that zooms the appearing view from a given source view.

