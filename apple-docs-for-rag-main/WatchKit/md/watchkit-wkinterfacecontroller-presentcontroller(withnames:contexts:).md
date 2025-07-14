

- WatchKit
- WKInterfaceController
-  presentController(withNames:contexts:) 

Instance Method

# presentController(withNames:contexts:)

Presents a page-based interface modally.

watchOS 2.0+

``` source
@MainActor
func presentController(
    withNames names: [String],
    contexts: [Any]?
)
```

## Parameters 

`names`  

An array of strings, each of which contains the name of an interface controller you want to display in the page-based interface. In your storyboard, the name of an interface controller is stored in the object’s Identifier property, which is located in the attributes inspector. The order of the strings in the array is used to set the order of the corresponding interface controllers. This parameter must not be `nil` or an empty array.

`contexts`  

An array of context objects to pass to the new interface controllers. Use the objects in this array to communicate important information to the new interface controllers, such as the data to display or any relevant state information. You may specify `nil` for this parameter, but doing so is not recommended.

Each object in the array is passed to the interface controller at the same index in the `names` parameter.

## Mentioned in 

Navigating Between Scenes

## Discussion

After calling this method, WatchKit loads and initializes the new interface controllers and animates them into position on top of the current interface controller. A modal interface slides up from the bottom of the screen and completely cover the previous interface. WatchKit displays the first interface controller in the `names` array initially. The user can navigate to the other interfaces by swiping horizontally.

The title of the modal interface is set to the string `Cancel` by default. Change the title using the setTitle(_:) method. Tapping the title dismisses the interface automatically. To dismiss the interface programmatically, call the dismiss() method.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Presenting interface controllers modally

func presentController(withName: String, context: Any?)

Presents a single interface controller modally.

func presentController(withNamesAndContexts: [(name: String, context: AnyObject)])

Presents a page-based interface modally.

func presentAlert(withTitle: String?, message: String?, preferredStyle: WKAlertControllerStyle, actions: [WKAlertAction])

Presents an alert or action sheet over the current interface controller.

enum WKAlertControllerStyle

Constants indicating the styles for standard system alerts.

func dismiss()

Dismisses the current interface controller from the screen.

