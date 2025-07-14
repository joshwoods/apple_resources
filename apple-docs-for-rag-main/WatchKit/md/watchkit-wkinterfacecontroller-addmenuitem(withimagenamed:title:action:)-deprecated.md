

- WatchKit
- WKInterfaceController
-  addMenuItem(withImageNamed:title:action:) Deprecated

Instance Method

# addMenuItem(withImageNamed:title:action:)

Adds an action to the context menu using an existing image resource in your Watch app bundle.

watchOS 2.0–7.0Deprecated

``` source
@MainActor
func addMenuItem(
    withImageNamed imageName: String,
    title: String,
    action: Selector
)
```

Deprecated

Elevate important items out of such menus and into the relevant screen or a settings screen.

## Parameters 

`imageName`  

The name of the image to be loaded from your Watch app’s bundle. Include the filename extension in the name. This parameter must not be `nil`.

`title`  

The title string to be displayed underneath the image. Title strings should be reasonably short. Any text that cannot be displayed is truncated. This parameter must not be `nil` or an empty string.

`action`  

The action method to be called when the action is tapped. The method must be defined on the current interface controller object. This parameter must not be `nil`.

## Discussion

Use this method to append an action to the interface controller’s context menu. If the menu already has four items, additional items are ignored.

## See Also

### Deprecated symbols

Text Response Key

Keys for retrieving text response information.

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

class func reloadRootControllers(withNames: [String], contexts: [Any]?)

Loads the specified interface controllers and rebuilds the app’s page-based interface.

Deprecated

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

enum WKMenuItemIcon

Template images that you can use for menus.

Deprecated

