

- UIKit
- UIAppearance
-  appearance(whenContainedInInstancesOf:) 

Type Method

# appearance(whenContainedInInstancesOf:)

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
static func appearance(whenContainedInInstancesOf containerTypes: [any UIAppearanceContainer.Type]) -> Self
```

**Required**

## Parameters 

`containerTypes`  

An array of appearance container classes, in ascending hierarchical order.

## Return Value

The appearance proxy to use for the object.

## Discussion

Set the `containerTypes` array to an ascending hierarchical list of containing types. For example, if you want a navigation bar to take on a specific appearance when contained in a navigation controller inside a tab bar controller, set `containerTypes` to `[UINavigationController.self, UITabBarController.self]` (Swift) or `@[[UINavigationController class], [UITabBarController class]]` (Objective-C).

Do not set `containerTypes` to an unrelated list of types or to a list that does not match the containment hierarchy of your user interface.

## See Also

### Working with the appearance proxy

static func appearance() -> Self

Returns the appearance proxy for the receiver.

**Required**

static func appearance(for: UITraitCollection) -> Self

Returns the appearance proxy for the receiver that has the passed trait collection.

**Required**

static func appearance(for: UITraitCollection, whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe and has the specified trait collection.

**Required**

