

- UIKit
- Mac Catalyst
-  Optimizing your iPad app for Mac 

Article

# Optimizing your iPad app for Mac

Make your iPad app more like a Mac app by taking advantage of system features in macOS.

## Overview

The Mac version of your iPad app supports many system features found in macOS without requiring any effort from you, including:

- A default menu bar for your app

- Support for trackpad, mouse, and keyboard input

- Support for window resizing and full-screen display

- Mac-style scroll bars

- Copy-and-paste support

- Drag-and-drop support

- Support for system Touch Bar controls

You can, however, extend your app to take advantage of even more system features.

Important

Mac apps built with Mac Catalyst can only use AppKit APIs marked as available in Mac Catalyst, such as NSToolbar and NSTouchBar. Mac Catalyst doesn’t support accessing unavailable AppKit APIs.

### Add menu bar items

The Mac version of your app comes with a standard menu bar. Customize it by adding and removing menu items using UIMenuBuilder. To learn more, see Adding menus and shortcuts to the menu bar and user interface.

### Show a Preferences window

Mac apps typically let users manage app-specific settings by displaying a Preferences window. Users see this window by selecting the app menu followed by the Preferences menu item in the menu bar. If your app has a Settings bundle, the system automatically provides your app with a preferences window. To learn more, see Displaying a Preferences window.

### Apply a translucent background to your primary view controller

iPad apps using a split view controller get a Mac-style vertical split view when running in macOS. But to make your iPad app look more at home on Mac, apply a translucent effect that blurs the desktop into the primary view controller’s background. To do this, set your split view controller’s primaryBackgroundStyle to UISplitViewController.BackgroundStyle.sidebar, as shown in the following code.

```
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {

    let splitViewController = window!.rootViewController as! UISplitViewController
    let navigationController = splitViewController.viewControllers[splitViewController.viewControllers.count-1] as! UINavigationController
    navigationController.topViewController!.navigationItem.leftBarButtonItem = splitViewController.displayModeButtonItem

    // Add a translucent background to the primary view controller.
    splitViewController.primaryBackgroundStyle = .sidebar

    splitViewController.delegate = self

    return true
}
```

### Detect the pointer in a view

Mac users rely on a pointer to interact with apps, whether selecting a text field or moving a window. As the user moves the pointer over UI elements, some elements should change their appearance. For example, a web browser highlights a link as the pointer moves over it.

To detect when the user moves the pointer over a view in your app, add a UIHoverGestureRecognizer to that view. This tells your app when the pointer enters or leaves the view, or moves while over it.

```
class ViewController: UIViewController {

    @IBOutlet var button: UIButton!

    override func viewDidLoad() {
        super.viewDidLoad()

        let hover = UIHoverGestureRecognizer(target: self, action: #selector(hovering(_:)))
        button.addGestureRecognizer(hover)
    }

    @objc
    func hovering(_ recognizer: UIHoverGestureRecognizer) {
        switch recognizer.state {
        case .began, .changed:
            button.titleLabel?.textColor = #colorLiteral(red: 1, green: 0, blue: 0, alpha: 1)
        case .ended:
            button.titleLabel?.textColor = UIColor.link
        default:
            break
        }
    }
}
```

## See Also

### App support

Bring an iPad App to the Mac with Mac Catalyst

Build a native Mac app from the same codebase as your iPad app.

Choosing a user interface idiom for your Mac app

Select the iPad or the Mac user interface idiom in your Mac app built with Mac Catalyst.

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

UIApplicationSupportsTabbedSceneCollection

A Boolean value indicating whether an app built with Mac Catalyst supports automatic tabbing mode.

