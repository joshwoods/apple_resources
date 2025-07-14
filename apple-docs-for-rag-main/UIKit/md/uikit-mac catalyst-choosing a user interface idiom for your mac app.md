

- UIKit
- Mac Catalyst
-  Choosing a user interface idiom for your Mac app 

Article

# Choosing a user interface idiom for your Mac app

Select the iPad or the Mac user interface idiom in your Mac app built with Mac Catalyst.

## Overview

A Mac app built with Mac Catalyst can run in either UIUserInterfaceIdiom.pad or UIUserInterfaceIdiom.mac user interface idioms. To choose the idiom in which your app runs, select from the following options after you turn on Mac Catalyst in your Xcode project:

Scale Interface to Match iPad  
Run your app in the UIUserInterfaceIdiom.pad idiom. Select this option to quickly bring your iPad app to the Mac.

Optimize Interface for Mac  
Run your app in the UIUserInterfaceIdiom.mac idiom. Select this option to show controls that look and behave like those available in AppKit.

Note

To learn more about turning on Mac Catalyst in your Xcode project, see Creating a Mac version of your iPad app.

### Start with the iPad idiom

By default, Xcode selects Scale Interface to Match iPad after you turn on Mac Catalyst. This option provides a simplified approach for bringing your iPad app to the Mac. Your Mac app runs in the UIUserInterfaceIdiom.pad idiom, which tells macOS to scale the app’s user interface to match the Mac display environment while preserving iPad-like appearance and view metrics.

When testing your app you may find that adopting controls that look and behave like those in AppKit or providing crisper-looking text can enhance the user experience of your app. If this is the case, change to the UIUserInterfaceIdiom.mac by selecting Optimize Interface for Mac. However, selecting this option may require you to make additional changes to your app.

### Update your app to use the Mac idiom

Choosing Optimize Interface for Mac means your Mac app runs in the UIUserInterfaceIdiom.mac user interface idiom, which changes the interface of your app. Some controls change their size and appearance, and interacting with them feels identical to interacting with AppKit controls. For example, UIButton appears identical to NSButton.

Because the system sets control sizes appropriately when the user interface idiom is UIUserInterfaceIdiom.mac, the system no longer needs to scale your app’s interface to match Mac sizing. Screen points are identical in size to those in AppKit-based apps. However, if your app has hard-coded sizes or uses images sized for iPad, you may need to update your app to accommodate the size differences. You may also need to adjust auto layout constraints.

Some controls provide additional settings that help you achieve a more Mac-like appearance. For instance, UISwitch can appear as a checkbox when idiom is UIUserInterfaceIdiom.mac by setting preferredStyle to UISwitch.Style.checkbox. Then set title to the text of the checkbox.

```
let showFavoritesAtTop = UISwitch()
showFavoritesAtTop.preferredStyle = .checkbox
if traitCollection.userInterfaceIdiom == .mac {
    showFavoritesAtTop.title = "Always show favorite recipes at the top"
}
```

UIPageControl, UIRefreshControl, and UIStepper aren’t available to apps running in the Mac idiom. If you attempt to display these controls in a view, your app throws an exception. Replace these controls with similar functionality when the user interface idiom is UIUserInterfaceIdiom.mac. For example, replace UIRefreshControl with a Refresh menu item by creating a UIKeyCommand object with the title “Refresh” and the keyboard shortcut Command-R. Then add the command to your app’s menu system. For more information, see Adding menus and shortcuts to the menu bar and user interface.

### Determine the current user interface idiom

To determine if your app is running in the Mac idiom, compare the value of the userInterfaceIdiom property with UIUserInterfaceIdiom.mac. When the comparison is true, you can tailor the behavior of your app for the Mac; for example, to display a different child view.

```
let childViewController: UIViewController
if traitCollection.userInterfaceIdiom == .mac {
    childViewController = MacOptimizedChildViewController()
} else {
    childViewController = ChildViewController()
}
addChild(childViewController)
childViewController.view.frame = view.bounds
view.addSubview(childViewController.view)
childViewController.didMove(toParent: self)
```

### Set the preferred behavioral style

When adopting the Mac idiom, some controls such as UIButton and UISlider appear identical to their AppKit counterparts. However, there may be situations where you want to take advantage of the Mac idiom in your app but keep a control’s iPad appearance and behavior. For instance, consider an iPad app that displays a slider with a custom thumb image. By default, the Mac version of the app, built with Mac Catalyst, displays a standard macOS slider when the user interface idiom is UIUserInterfaceIdiom.mac.

To provide a slider with an appearance that’s consistent in both iPad and Mac versions of the app, set the preferredBehavioralStyle of the slider to UIBehavioralStyle.pad. This behavioral style tells the slider to behave as if the user interface idiom is UIUserInterfaceIdiom.pad even though the app is using the Mac idiom.

Remember, macOS doesn’t scale the interface of apps that use the Mac idiom so you may need to update your app to accommodate size differences even when the preferred behavioral style is UIBehavioralStyle.pad. For example, a slider with a custom thumb image may need an image of a different size for the Mac app than the one used in the iPad app.

```
let slider = UISlider()
slider.minimumValue = 0
slider.maximumValue = 1
slider.value = 0.5
slider.preferredBehavioralStyle = .pad

if slider.traitCollection.userInterfaceIdiom == .mac {
    slider.setThumbImage(#imageLiteral(resourceName: "customSliderThumbMac"), for: .normal)
} else {
    slider.setThumbImage(#imageLiteral(resourceName: "customSliderThumb"), for: .normal)
}
```

There are some properties and methods of UIButton and UISlider not supported in the Mac idiom when the behavioral style is UIBehavioralStyle.mac, and calling these throws an exception; for example, setting a button’s title or image for any control state other than normal, and setting a slider’s thumb image, minimum or maximum track image, tint color, or value image. However, these properties and methods are available for use in the Mac idiom when the control’s behavioral style is UIBehavioralStyle.pad.

### Provide a different code path

Even when your Mac app runs in the UIUserInterfaceIdiom.pad idiom, you may need to change the appearance or behavior of your Mac app. Use the `targetEnvironment()` compilation conditional to choose a different code path depending on the target environment.

For example, if your iPad app displays a delete item confirmation in a popover next to a delete button but you want to display the confirmation as an alert in your Mac app, add a `targetEnvironment()` conditional to determine the preferred style of the alert controller.

```
let deleteAction = UIAlertAction(title: "Delete", style: .destructive) { (action) in
    if dataStore.delete(recipe) {
        self.recipe = nil
    }
}

let cancelAction = UIAlertAction(title: "Cancel", style: .cancel, handler: nil)

#if targetEnvironment(macCatalyst)
let preferredStyle = UIAlertController.Style.alert
#else
let preferredStyle = UIAlertController.Style.actionSheet
#endif

let alert = UIAlertController(title: "Are you sure you want to delete \(recipe.title)?", message: nil, preferredStyle: preferredStyle)
alert.addAction(deleteAction)
alert.addAction(cancelAction)

if let popoverPresentationController = alert.popoverPresentationController {
    popoverPresentationController.barButtonItem = sender as? UIBarButtonItem
}

present(alert, animated: true, completion: nil)
```

## See Also

### App support

Bring an iPad App to the Mac with Mac Catalyst

Build a native Mac app from the same codebase as your iPad app.

Optimizing your iPad app for Mac

Make your iPad app more like a Mac app by taking advantage of system features in macOS.

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

UIApplicationSupportsTabbedSceneCollection

A Boolean value indicating whether an app built with Mac Catalyst supports automatic tabbing mode.

