

- UIKit
- UIInputViewController
-  needsInputModeSwitchKey 

Instance Property

# needsInputModeSwitchKey

A Boolean value that indicates whether the keyboard must display an input switcher key.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var needsInputModeSwitchKey: Bool { get }
```

## Discussion

The input switcher key allows the user to switch between different keyboards. When this property is true, your custom keyboard should provide such a key.

## See Also

### Configuring the keyboard behaviors

var hasFullAccess: Bool

A Boolean value that indicates whether the keyboard has full access.

var hasDictationKey: Bool

A Boolean value that indicates whether the keyboard has a dictation key.

