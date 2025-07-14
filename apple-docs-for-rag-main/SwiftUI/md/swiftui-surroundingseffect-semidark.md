

- SwiftUI
- SurroundingsEffect
-  semiDark 

Type Property

# semiDark

An effect that dims passthrough video less than dark.

visionOS 2.0+

``` source
static var semiDark: SurroundingsEffect { get }
```

## Discussion

Use this value with the preferredSurroundingsEffect(_:) view modifier when you want to dim passthrough video while displaying a particular view. Doing so helps to draw attention to your app’s content while still enabling people to remain aware of their surroundings. This value can be used in the shared space.

