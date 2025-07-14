

- WatchKit
- WKInterfaceController
-  dismiss() 

Instance Method

# dismiss()

Dismisses the current interface controller from the screen.

watchOS 2.0+

``` source
@MainActor
func dismiss()
```

## Discussion

Call this method when you want to dismiss an interface controller that you presented modally. Always call this method from your WatchKit extension’s main thread.

## See Also

### Presenting interface controllers modally

func presentController(withName: String, context: Any?)

Presents a single interface controller modally.

func presentController(withNames: [String], contexts: [Any]?)

Presents a page-based interface modally.

func presentController(withNamesAndContexts: [(name: String, context: AnyObject)])

Presents a page-based interface modally.

func presentAlert(withTitle: String?, message: String?, preferredStyle: WKAlertControllerStyle, actions: [WKAlertAction])

Presents an alert or action sheet over the current interface controller.

enum WKAlertControllerStyle

Constants indicating the styles for standard system alerts.

