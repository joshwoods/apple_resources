

- Safari Services
- Safari app extensions
- Safari app extension information property list keys
-  Adjusting settings for a toolbar item 

Article

# Adjusting settings for a toolbar item

Customize a toolbar item for your Safari app extension.

## Overview

Safari has a user-customizable toolbar that can contain a selection of buttons. A Safari app extension can provide a new toolbar item, and when the Safari app extension is in an enabled state, Safari adds that item to the toolbar by default. The user may choose to hide your toolbar item by customizing the toolbar.

Your app extension can enable or disable the toolbar item or add a badge with text to it. When the user clicks it, the toolbar item can either execute a command or display a popover. The decision of which behavior to implement occurs at design time. For more information, see Display a popover for a toolbar item.

Add a toolbar item with the following steps:

1.  Create an image.

2.  Fill out the appropriate fields in the `Info.plist` file.

3.  Add logic that executes when the user clicks the toolbar button.

To learn how to add a toolbar item, see Using contextual menu and toolbar item keys.

### Localize the toolbar label

Provide an `InfoPlist.strings` file and include localized text for a custom key based on your toolbar identifier. For example, to provide a Polish translation for a toolbar item with an identifier of `translate`, add the following entry to your strings file:

```
"Toolbar Button Label for Identifier: translate" = "Przetłumacz";
```

For more information, see Managing Your App’s Information Property List.

### Dynamically change the image of a toolbar item

To update a toolbar item’s image dynamically, Safari uses the setImage(_:) method for `SFSafariToolbarItem`. Setting the image to `nil` sets the default image.

### Adjust the state of the toolbar item

Your app extension has the following control over the toolbar item:

- The app extension can enable or disable the button. Use setEnabled(_:) if your toolbar item is usable only some of the time.

- The app extension can add a string to the toolbar item as a badge. For example, if your extension contains a list of items that the user can see by clicking the button, you might add a badge to the toolbar item using setBadgeText(_:) with the number of unread items.

State changes can trigger in either of the following ways:

- Based on the user’s actions, Safari can implement a change to the button’s state.

- Your app extension can force a state change to happen explicitly.

Important

An injected content script can’t directly force the toolbar item to become enabled or disabled. However, you can implement this control yourself by sending a message to your app extension, and changing the toolbar state in your message handler. For more information, see Passing messages between Safari app extensions and injected scripts.

### Validate the Safari toolbar item

When an event occurs that may require your toolbar’s state to change, Safari calls your app extension’s event handler. The event handler receives parameters that indicate the window the toolbar appears in, and a completion handler for your app extension to call. Your event handler determines whether to enable or disable the toolbar button and whether to display a badge, and then returns this information to Safari.

The code below shows one possible implementation of the validateToolbarItem(in:validationHandler:)method. In this case, the app extension has a list of items that it keeps track of, and it adds a badge to the toolbar item with the number of available items.

- Swift
- Objective-C

```
override func validateToolbarItem(in window: SFSafariWindow, validationHandler: ((Bool, String) -> Void)) {
    // The system calls this when Safari's state changes in a way that requires revalidation of the extension's toolbar item.
    if items.count == 0
    {
        validationHandler(false,"")
    }
    else
    {
        validationHandler(true,"\(items.count)")
    }
}
```

```
- (void)validateToolbarItemInWindow:(SFSafariWindow *)window validationHandler:(void (^)(BOOL enabled, NSString *badgeText))validationHandler {
    // The system calls this when Safari's state changes in a way that requires revalidation of the extension's toolbar item.
    if (self.items.count == 0)
    {
        validationHandler(NO,nil);
    }
    else
    {
        validationHandler(YES, [NSString stringWithFormat:@"%lu", (unsigned long)self.items.count] );
    }
}
```

### Set the toolbar information explicitly

If you have a reference to an SFSafariWindow object, you can use it to get a proxy object for the toolbar item, and then use that object to set the toolbar’s status directly.

- Swift
- Objective-C

```
override func toolbarItemClicked(in window: SFSafariWindow) {
    window.getToolbarItem { (toolbarItem) in
        toolbarItem?.setEnabled(true, withBadgeText: "1")
    }
}
```

```
- (void)toolbarItemClickedInWindow:(SFSafariWindow *)window
{
    [window getToolbarItemWithCompletionHandler:^(SFSafariToolbarItem *toolbarItem)
     {
         [toolbarItem setEnabled:NO withBadgeText:@"1"];
     }];
}
```

### Add commands to the toolbar item

If you configure your toolbar item to send a command, clicking the toolbar button in Safari calls your extension handler’s toolbarItemClicked(in:) method. You can then process the event however you like. The window passes in as a parameter, so this code retrieves the toolbar item for that window and updates its badge.

Another common usage when the toolbar item activates is to forward the message to an injected script on the page, so that you can modify the page in some way. The code below shows one possible way to forward the toolbar action. This code retrieves the active tab on the window that the user clicks, uses the tab to retrieve the page, and then dispatches a message to the page.

- Swift
- Objective-C

```
window.getActiveTab { (activeTab) in
    activeTab?.getActivePage { (activePage) in
        activePage?.dispatchMessageToScript(withName: "DoSomethingInteresting", userInfo: nil)
    }
}
```

```
[window getActiveTabWithCompletionHandler:^(SFSafariTab *activeTab) {
    [activeTab getActivePageWithCompletionHandler:^(SFSafariPage *activePage) {
        [activePage dispatchMessageToScriptWithName:@"DoSomethingInteresting" userInfo:nil];
    }];
}];
```

### Display a popover for a toolbar item

A popover is a window that pops up over an active window when the user clicks a toolbar button — no navigation is necessary. You can use a popover to show a small amount of information or to complete a small action. The popover closes automatically when the user changes focus (by clicking another window, for example). The Human Interface Guidelines describe how to best use popovers.

In a Safari app extension, you implement the popover content using native view and view controller objects based on AppKit. When your native app and your Safari app extension share the same data model, this design also makes it easier to share other pieces of view code between the two. Safari and the operating system do all of the work to display this content within the Safari browser and to process events as they come in.

You implement your popover as a subclass of SFSafariExtensionViewController. As with other macOS development, typically you add your own outlets and actions to the view controller, and provide an XIB file for its user interface. The Xcode template for a Safari app extension provides some boilerplate code to get you started. Use Auto Layout so that your content adapts to different sizes.

If you configure your toolbar item to display a popover, clicking the toolbar button in Safari calls your extension handler’s popoverViewController() method. Your app extension instantiates and returns the popover view controller. In the template, the popover implements as a singleton object.

- Swift
- Objective-C

```
override func popoverViewController() -> SFSafariExtensionViewController {
    return SafariExtensionViewController.shared
}

```

```
- (SFSafariExtensionViewController *)popoverViewController {
    return [SafariExtensionViewController sharedController];
}
```

Before displaying the popover, the system calls your handler’s popoverWillShow(in:) method. You can use this method to populate the contents of the window with new information. Similarly, after the popover disappears, the system calls the handler’s popoverDidClose(in:) method so that you can perform any necessary cleanup.

## See Also

### Contextual menu and toolbar items

Using contextual menu and toolbar item keys

Learn about adding contextual menu items and toolbar items to a Safari app extension with information property list keys.

Adjusting settings for contextual menu items

Customize contextual menu items for your Safari app extension.

class SFSafariToolbarItem

A proxy for a Safari app extension toolbar item in a Safari window.

class SFSafariExtensionViewController

The view controller for a popover associated with your app extension.

