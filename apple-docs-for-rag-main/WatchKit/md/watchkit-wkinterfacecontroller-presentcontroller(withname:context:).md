

- WatchKit
- WKInterfaceController
-  presentController(withName:context:) 

Instance Method

# presentController(withName:context:)

Presents a single interface controller modally.

watchOS 2.0+

``` source
@MainActor
func presentController(
    withName name: String,
    context: Any?
)
```

## Parameters 

`name`  

The name of the interface controller you want to display. In your storyboard, the name of an interface controller is stored in the object’s Identifier property, which is located in the attributes inspector. This parameter must not be `nil`.

`context`  

An object to pass to the new interface controller. Use the object in this parameter to communicate important information to the new interface controller, such as the data to display or any relevant state information. You may specify `nil` for this parameter, but doing so is not recommended.

## Mentioned in 

Navigating Between Scenes

## Discussion

After calling this method, the WatchKit extension loads and initializes the new interface controller and animates it into position on top of the current interface controller. A modal interface slides up from the bottom of the screen and completely covers the previous interface.

The title of the modal interface is set to the string `Cancel` by default. Change the title using the setTitle(_:) method. Tapping the title dismisses the interface automatically. To dismiss the interface programmatically, call the dismiss() method.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Presenting interface controllers modally

func presentController(withNames: [String], contexts: [Any]?)

Presents a page-based interface modally.

func presentController(withNamesAndContexts: [(name: String, context: AnyObject)])

Presents a page-based interface modally.

func presentAlert(withTitle: String?, message: String?, preferredStyle: WKAlertControllerStyle, actions: [WKAlertAction])

Presents an alert or action sheet over the current interface controller.

enum WKAlertControllerStyle

Constants indicating the styles for standard system alerts.

func dismiss()

Dismisses the current interface controller from the screen.

