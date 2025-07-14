

- WatchKit
- WKInterfaceController
-  reloadRootControllers(withNames:contexts:) Deprecated

Type Method

# reloadRootControllers(withNames:contexts:)

Loads the specified interface controllers and rebuilds the app’s page-based interface.

watchOS 2.0–4.0Deprecated

``` source
@MainActor
class func reloadRootControllers(
    withNames names: [String],
    contexts: [Any]?
)
```

Deprecated

Use reloadRootPageControllers(withNames:contexts:orientation:pageIndex:) instead.

## Parameters 

`names`  

An array of NSString objects, each of which contains the identifier of an interface controller in your storyboard file. The order of the identifiers in the array defines the order of the corresponding interface controllers in the page-based interface.

`contexts`  

An array of objects of type `id`. Use this parameter to pass context objects to each of the interface controllers loaded into the page-based interface. The first object in the array is passed to the first interface controller, the second object is passed to the second interface controller, and so on.

## Discussion

Call this method to reload the pages in your app’s page-based interface:

- **At launch time.** Use this method to customize the set of pages you want displayed.

- **At runtime.** Use it to change the active set of pages, adding or removing pages as needed.

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

func presentController([(name: String, context: AnyObject)])

Presents a page-based interface modally.

Deprecated

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

enum WKMenuItemIcon

Template images that you can use for menus.

Deprecated

