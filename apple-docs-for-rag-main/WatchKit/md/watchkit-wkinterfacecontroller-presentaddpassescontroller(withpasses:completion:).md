

- WatchKit
- WKInterfaceController
-  presentAddPassesController(withPasses:completion:) 

Instance Method

# presentAddPassesController(withPasses:completion:)

Displays a modal interface for presenting passes to the user.

watchOS 2.0+

``` source
@MainActor
func presentAddPassesController(
    withPasses passes: [PKPass],
    completion: @escaping () -> Void
)
```

``` source
@MainActor
func presentAddPassesController(withPasses passes: [PKPass]) async
```

## Parameters 

`passes`  

An array of PKPass objects that you want to present to the user.

`completion`  

The block to execute when the user is ready to dismiss the interface. Use this block to perform any cleanup tasks related to the dismissal of the modal interface. This block has no return value and takes no parameters.

## Mentioned in 

Navigating Between Scenes

## Discussion

Use this method to display PassKit passes to the user and to give the user the option to add them to their pass library. This method executes asynchronously, returning shortly after you call it. During a subsequent run loop cycle, the system displays the pass interface over the current interface controller. Always call this method from your WatchKit extension’s main thread.

The user dismisses the interface using the built-in controls. At dismissal time, the interface controller executes your `completion` block so that you can perform any relevant cleanup tasks.

## See Also

### Adding PassKit passes

func dismissAddPassesController()

Dismisses the pass interface controller

