

- WatchKit
- WKInterfaceController
-  popToRootController() 

Instance Method

# popToRootController()

Pops all interface controllers except the app’s initial interface controller.

watchOS 2.0+

``` source
@MainActor
func popToRootController()
```

## Discussion

Use this method to return your interface to its initial configuration. You might do this so that you can reset your navigation hierarchy to its initial state before pushing one or more different interface controllers onto the navigation stack.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Implementing a navigation interface

func pushController(withName: String, context: Any?)

Pushes a new interface controller onto the screen.

func pop()

Pops the current interface controller from the screen.

