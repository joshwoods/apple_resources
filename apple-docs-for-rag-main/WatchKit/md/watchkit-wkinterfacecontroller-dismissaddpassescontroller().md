

- WatchKit
- WKInterfaceController
-  dismissAddPassesController() 

Instance Method

# dismissAddPassesController()

Dismisses the pass interface controller

watchOS 2.0+

``` source
@MainActor
func dismissAddPassesController()
```

## Discussion

Use this method to dismiss a pass controller you previously displayed using the presentAddPassesController(withPasses:completion:) method. When dismissing the pass controller programmatically, WatchKit still calls the completion block you provided.

## See Also

### Adding PassKit passes

func presentAddPassesController(withPasses: [PKPass], completion: () -> Void)

Displays a modal interface for presenting passes to the user.

