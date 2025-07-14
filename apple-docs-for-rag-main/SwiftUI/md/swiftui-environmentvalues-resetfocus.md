

- SwiftUI
- EnvironmentValues
-  resetFocus 

Instance Property

# resetFocus

An action that requests the focus system to reevaluate default focus.

macOS 12.0+tvOS 14.0+watchOS 7.0+

``` source
var resetFocus: ResetFocusAction { get }
```

## Discussion

Get this environment value and call and call it as a function to force a default focus reevaluation at runtime.

```
@Namespace var mainNamespace
@Environment(\.resetFocus) var resetFocus

var body: some View {
    // ...
    resetFocus(in: mainNamespace)
    // ...
}
```

## See Also

### Resetting focus

struct ResetFocusAction

An environment value that provides the ability to reevaluate default focus.

