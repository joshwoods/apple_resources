

- SwiftUI
-  ResetFocusAction 

Structure

# ResetFocusAction

An environment value that provides the ability to reevaluate default focus.

macOS 12.0+tvOS 14.0+watchOS 7.0+

``` source
struct ResetFocusAction
```

## Overview

Get the resetFocus environment value and call it as a function to force a default focus reevaluation at runtime.

```
@Namespace var mainNamespace
@Environment(\.resetFocus) var resetFocus

var body: some View {
    // ...
    resetFocus(in: mainNamespace)
    // ...
}
```

## Topics

### Calling the action

func callAsFunction(in: Namespace.ID)

Asks the focus sytem to reevaluate the default focus item.

## See Also

### Resetting focus

var resetFocus: ResetFocusAction

An action that requests the focus system to reevaluate default focus.

