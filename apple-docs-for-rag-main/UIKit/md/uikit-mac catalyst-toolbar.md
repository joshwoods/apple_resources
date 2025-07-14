

- UIKit
- Mac Catalyst
-  Toolbar 

API Collection

# Toolbar

Provide a space for controls under a window’s title bar and above your custom content.

## Topics

### View

Integrating a Toolbar and Touch Bar into Your App

Provide users quick access to your app’s features from a toolbar and corresponding Touch Bar.

@MainActor class NSToolbar

An object that manages the space above your app’s custom content and either below or integrated with the window’s title bar.

protocol NSToolbarItemValidation : NSObjectProtocol

Validation of a toolbar item.

### Items

@MainActor class NSToolbarItem

A single item that appears in a window’s toolbar.

@MainActor class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

@MainActor class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

@MainActor class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

@MainActor class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

class NSUIViewToolbarItem

An item in a window’s toolbar that hosts a custom UIKit view.

### Item validation

protocol NSCloudSharingValidation : NSObjectProtocol

A protocol that a Cloud-sharing toolbar item uses to get validation of an item.

## See Also

### User interface

UIKit Catalog: Creating and customizing views and controls

Customize your app’s user interface with views and controls.

Building and improving your app with Mac Catalyst

Improve your iPadOS app with Mac Catalyst by supporting native controls, multiple windows, sharing, printing, menus and keyboard shortcuts.

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

Removing the title bar in your Mac app built with Mac Catalyst

Display content that fills the entire height of a window by removing the title bar.

Touch Bar

Display interactive content and controls in the Touch Bar.

