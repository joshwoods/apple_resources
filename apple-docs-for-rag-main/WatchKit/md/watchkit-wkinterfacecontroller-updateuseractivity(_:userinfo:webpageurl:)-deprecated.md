

- WatchKit
- WKInterfaceController
-  updateUserActivity(\_:userInfo:webpageURL:) Deprecated

Instance Method

# updateUserActivity(\_:userInfo:webpageURL:)

Registers the current user activity with the system.

watchOS 2.0–5.0Deprecated

``` source
@MainActor
func updateUserActivity(
    _ type: String,
    userInfo: [AnyHashable : Any]? = nil,
    webpageURL: URL?
)
```

Deprecated

Use update(_:) instead.

## Parameters 

`type`  

The type of activity to be continued. The value is a developer-defined string in reverse-DNS format by convention, for example, `com.myCompany.myEditor.editing`. This parameter must not be `nil` or an empty string.

`userInfo`  

A dictionary containing app-specific state information needed to continue an activity on another device. Keys and values in the dictionary must be of the following types: NSArray, NSData, NSDate, NSDictionary, NSNull, NSNumber, NSSet, or NSString.

`webpageURL`  

A URL containing the web page to load in a browser to continue the activity. The scheme of the URL must be `http` or `https`. Any other scheme throws an exception.

## Discussion

Use this method to publish your app’s current activity so that it can be handled as needed. When calling this method, you must specify a value for the `userInfo` parameter, the `webpageURL` parameter, or both. Call this method in the following situations:

- In your glance interface controller, call this method and provide a `userInfo` dictionary with information about what the glance displays. If the user taps your glance, that contextual information passes to your app so it can configure its interface.

- Call this method to register the current activity with Handoff. The system delivers the information to the user’s iPhone, which can propagate the Handoff information to the user’s other devices. For more information about supporting Handoff, see Handoff Programming Guide.

Call this method at any time during the execution of your interface controller’s code. The system takes the information you provide and stores it for delivery to the appropriate target.

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

class func reloadRootControllers(withNames: [String], contexts: [Any]?)

Loads the specified interface controllers and rebuilds the app’s page-based interface.

Deprecated

enum WKMenuItemIcon

Template images that you can use for menus.

Deprecated

