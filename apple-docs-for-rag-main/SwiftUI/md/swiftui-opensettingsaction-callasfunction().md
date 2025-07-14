

- SwiftUI
- OpenSettingsAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Opens the window associated to the Settings scene defined by this app, if one exists.

macOS 14.0+

``` source
@MainActor @preconcurrency
func callAsFunction()
```

## Discussion

Calling this action when the window is already open will order it to the front.

Don’t call this method directly. SwiftUI calls it when you call the openSettings action:

```
openSettings()
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

