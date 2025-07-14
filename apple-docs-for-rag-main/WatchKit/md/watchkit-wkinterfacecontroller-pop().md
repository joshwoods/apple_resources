

- WatchKit
- WKInterfaceController
-  pop() 

Instance Method

# pop()

Pops the current interface controller from the screen.

watchOS 2.0+

``` source
@MainActor
func pop()
```

## Mentioned in 

Navigating Between Scenes

## Discussion

After pushing an interface controller onto the screen, use this method to remove it and display the previous interface controller again. The system animates the transition back to the previous interface controller asynchronously.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Implementing a navigation interface

func pushController(withName: String, context: Any?)

Pushes a new interface controller onto the screen.

func popToRootController()

Pops all interface controllers except the app’s initial interface controller.

