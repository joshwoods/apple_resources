

- SwiftUI
- SurroundingsEffect
-  ultraDark 

Type Property

# ultraDark

An effect that dims passthrough video more than dark

visionOS 2.0+

``` source
static var ultraDark: SurroundingsEffect { get }
```

## Discussion

Use this value with the preferredSurroundingsEffect(_:) view modifier when you want to dim passthrough video while displaying a particular view. Doing so helps to draw attention to your app’s content while still enabling people to remain aware of their surroundings. This effect will only be applied while an immersive space is opened.

