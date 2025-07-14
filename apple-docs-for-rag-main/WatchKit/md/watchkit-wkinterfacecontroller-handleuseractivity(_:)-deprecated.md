

- WatchKit
- WKInterfaceController
-  handleUserActivity(\_:) Deprecated

Instance Method

# handleUserActivity(\_:)

Responds to Handoff–related activity.

watchOS 2.0–4.0Deprecated

``` source
@MainActor
func handleUserActivity(_ userInfo: [AnyHashable : Any]?)
```

Deprecated

Use the WKExtensionDelegate protocol’s handleUserActivity(_:) method instead.

## Parameters 

`userInfo`  

The dictionary containing data about the activity. When launching an app from its glance, WatchKit sets this parameter to the dictionary that the glance passed to the updateUserActivity(_:userInfo:webpageURL:) method.

## Discussion

Implement this method in your app’s initial interface controller and use it to respond to Handoff–related activity. If you do not implement the handleUserActivity(_:) method in your app’s extension delegate, WatchKit calls this method on your app’s initial interface controller. (If your app uses a page-based interface, WatchKit calls this method for each interface controller that is part of your initial interface.) Your implementation of this method should look at the `userInfo` dictionary and decide what actions (if any) to take. For example, an interface controller in a page-based interface might make itself the current page.

The default implementation of this method does nothing. When overriding this method, do not call `super`.

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

func presentController([(name: String, context: AnyObject)])

Presents a page-based interface modally.

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

