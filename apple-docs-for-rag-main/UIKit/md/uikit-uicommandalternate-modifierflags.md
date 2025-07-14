

- UIKit
- UICommandAlternate
-  modifierFlags 

Instance Property

# modifierFlags

The bit mask of modifier keys that the user must press to invoke the action for the alternative command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var modifierFlags: UIKeyModifierFlags { get }
```

## See Also

### Getting information about the alternative

var title: String

The command alternative’s title.

var action: Selector

The command alternative’s action-method selector.

