

- WatchKit
- WKInterfaceController
-  presentController(\_:) Deprecated

Instance Method

# presentController(\_:)

Presents a page-based interface modally.

iOS 8.2+iPadOS 8.2+watchOS

``` source
@MainActor @nonobjc @preconcurrency
final func presentController(_ namesAndContexts: [(name: String, context: AnyObject)])
```

Deprecated

Use presentController(withNamesAndContexts:) instead.

## Parameters 

`namesAndContexts`  

An array of tuples. Each tuple must contain the following named elements:

name  
The name of the interface controller you want to display. In your storyboard, the name of an interface controller is stored in the object’s Identifier property, which is located in the attributes inspector. This element must not be `nil`.

context  
An object to pass to the new interface controller. Use the object in this parameter to communicate important information to the new interface controller, such as the data to display or any relevant state information. You may specify `nil` for this element if you want but doing so is not recommended.

## Discussion

After calling this method, WatchKit loads and initializes the new interface controllers and animates them into position on top of the current interface controller. A modal interface slides up from the bottom of the screen and completely cover the previous interface. WatchKit displays the first interface controller in the `names` array initially. The user can navigate to the other interfaces by swiping horizontally.

The title of the modal interface is set to the string Cancel unless the presented interface controller explicitly changes it using the setTitle(_:) method. Tapping the title dismisses the interface automatically. To dismiss the interface programmatically, call the dismiss() method.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Deprecated symbols

Text Response Key

Keys for retrieving text response information.

func addMenuItem(withImageNamed: String, title: String, action: Selector)

Adds an action to the context menu using an existing image resource in your Watch app bundle.

Deprecated

func addMenuItem(with: WKMenuItemIcon, title: String, action: Selector)

Adds an action to the context menu using a system-provided icon.

Deprecated

func addMenuItem(with: UIImage, title: String, action: Selector)

Adds an action to the context menu by using an image provided by your WatchKit extension.

Deprecated

func beginGlanceUpdates()

Tells the system that you are about to start a potentially lengthy update task for your glance.

Deprecated

func clearAllMenuItems()

Removes all programmatically added actions from the context menu.

Deprecated

func endGlanceUpdates()

Tells the system that you finished updating your glance content.

Deprecated

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity.

Deprecated

class func reloadRootControllers(withNames: [String], contexts: [Any]?)

Loads the specified interface controllers and rebuilds the app’s page-based interface.

Deprecated

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

enum WKMenuItemIcon

Template images that you can use for menus.

Deprecated

