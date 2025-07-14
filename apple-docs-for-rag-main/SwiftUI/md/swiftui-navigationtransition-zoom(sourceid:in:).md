

- SwiftUI
- NavigationTransition
-  zoom(sourceID:in:) 

Type Method

# zoom(sourceID:in:)

A navigation transition that zooms the appearing view from a given source view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func zoom(
    sourceID: some Hashable,
    in namespace: Namespace.ID
) -> ZoomNavigationTransition
```

Available when `Self` is `ZoomNavigationTransition`.

## Parameters 

`sourceID`  

The identifier you provide to a corresponding `matchedTransitionSource` modifier.

`namespace`  

The namespace where you define the `id`. You can create new namespaces by adding the Namespace attribute to a View type, then reading its value in the view’s body method.

## Discussion

Indicate the source view using the `View/matchedTransitionSource(id:namespace:)` modifier.

## See Also

### Getting built-in transitions

static var automatic: AutomaticNavigationTransition

A style that automatically chooses the appropriate presentation transition for the current context.

