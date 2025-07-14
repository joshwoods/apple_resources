

- UIKit
- UIFocusItem
-  focusEffect 

Instance Property

# focusEffect

The visual effect to apply when the item becomes focused.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
optional var focusEffect: UIFocusEffect? { get }
```

## Discussion

A `nil` value indicates that the system shouldn’t apply any visual effects when the item becomes focused.

If you don’t implement this property, its value is `nil`.

