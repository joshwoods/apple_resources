

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  modifierKeyAlternate(\_:\_:) 

Instance Method

# modifierKeyAlternate(\_:\_:)

Builds a view to use in place of the modified view when the user presses the modifier key(s) indicated by the given set.

RealityKitSwiftUImacOS 15.0+

``` source
nonisolated
func modifierKeyAlternate(
    _ modifiers: EventModifiers,
    @ViewBuilder _ alternate: () -> V
) -> some View where V : View
```

## Parameters 

`modifiers`  

The modifier keys to associate with the alternate view. While all these keys are held, SwiftUI will replace the modified view with this alternate one.

`alternate`  

A view builder for constructing the modified view’s alternate when matching modifier keys are pressed.

## Return Value

A modified view with an alternate view to use while specific modifier keys are held down.

## Discussion

```
Button("Go Forward", ...)
    .modifierKeyAlternate(.option) {
        Button("Go to Page…", ...)
    }
```

In menu style contexts, modifier key alternates become alternate menu items. If the modified view has a keyboard shortcut, it will be used as the basis for the alternate view’s shortcut.

```
// File > Save
Button("Save", ...) // ⌘ S
    .keyboardShortcut("s")
    .modifierKeyAlternate(.option) {
        Button("Save All", ...) // ⌥⌘ S
    }
```

To use a different keyboard shortcut for the alternate view, add one explicitly in the view builder. SwiftUI will use your explicit shortcut instead of its own inferred one.

```
Button("Go Forward", ...) // ⌘ →
    .keyboardShortcut(.rightArrow)
    .modifierKeyAlternate(.control) {
        Button("Go To Page…", ...) // ⌃ →
            .keyboardShortcut(.rightArrow, modifiers: .control)
    }
```

A view can have multiple modifier key alternates, provided their associated modifier keys are different. When multiple alternates match the currently-held keys, the most specific match prevails.

```
Button("Save", ...) // ⌘ S
    .keyboardShortcut("s")
    .modifierKeyAlternate(.option) {
        Button("Save All", ...) // ⌥⌘ S
    }
    .modifierKeyAlternate([.option, .shift]) {
        Button("Save a Copy…", ...) // ⇧⌥⌘ S
    }
```

