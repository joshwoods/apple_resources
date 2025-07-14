

- WatchKit
- WKInterfaceController
-  beginGlanceUpdates() Deprecated

Instance Method

# beginGlanceUpdates()

Tells the system that you are about to start a potentially lengthy update task for your glance.

watchOS 2.0–4.0Deprecated

``` source
@MainActor
func beginGlanceUpdates()
```

Deprecated

watchOS no longer supports glances.

## Discussion

Calling this method is not required when updating your glance. This method is intended for situations where loading your glance content involves asynchronous method calls or other potentially lengthy tasks. Calling it from your willActivate() method before you start such operations causes WatchKit to continue displaying the glance loading screen until you call the endGlanceUpdates() method. Even if your glance is not yet onscreen, calling this method gives you extra time to process results received from an asynchronous call.

You must balance each call to this method with a corresponding call to the endGlanceUpdates() method. Failure to do so prevents your updated glance content from being displayed. You may nest calls to this method to mark several update points. When the willActivate() method returns, WatchKit checks for any in-progress glance updates and displays the loading screen until you make the matching calls to the endGlanceUpdates() method.

When your interface controller’s didDeactivate() method is called, WatchKit ends any outstanding glance updates automatically.

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

func clearAllMenuItems()

Removes all programmatically added actions from the context menu.

Deprecated

func endGlanceUpdates()

Tells the system that you finished updating your glance content.

Deprecated

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity.

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

