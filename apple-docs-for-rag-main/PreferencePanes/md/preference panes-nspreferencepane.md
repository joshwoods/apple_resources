

- Preference Panes
-  NSPreferencePane 

Class

# NSPreferencePane

The interface for providing preference panes to System Preferences or other apps.

Mac Catalyst 14.0+macOS 10.1+

``` source
class NSPreferencePane
```

## Overview

Preference panes are subclasses of NSPreferencePane, packaged up in bundles and loaded by a preference application, such as System Preferences. These bundles have a suffix of `.prefPane`. Bundles intended for use by System Preferences are located in the `Library/PreferencePanes` directories of the various file system domains. See the chapter About the macOS File System in File System Programming Guide for information about domains.

The preference pane bundle normally contains a nib file with the user interface for modifying user preferences. The nib file contains a window assigned to the \_window outlet of the preference pane instance (the nib’s File’s Owner). The `NSPreferencePane` implementation of loadMainView(), invoked by the preference application, loads the nib file and uses the content view of \_window as the preference pane’s main view. Override this method if you need a different technique for creating the user interface.

The NSPreferencePane subclass is responsible for initializing the user interface with the current preference settings and recording any modifications the user makes. Through a series of `will...`, `did...`, and `should...` methods, the preference application notifies the preference pane when the pane is selected (displayed) and deselected, allowing the pane to perform the necessary actions at the appropriate times. Implement these methods (and any additional target-action methods connected to the interface) as needed to produce the desired behavior for your preference pane.

Preference panes support Help menu items. Specify global help menu items in your bundle’s `Info.plist` file under the `NSPrefPaneHelpAnchors` key. To add dynamic help items, implement the updateHelpMenu(with:) method.

## Topics

### Initializing the Preference Pane

init(bundle: Bundle)

Initializes a preference pane with the specified bundle.

### Loading the Main View

func loadMainView() -> NSView

Loads the preference pane’s user interface into its main view.

func assignMainView()

Locates and assigns the preference pane’s main view from the nib file loaded by loadMainView().

func mainViewDidLoad()

Notifies the preference pane that the main view is set up and prepared to be displayed.

### Getting the Bundle Information

var bundle: Bundle

The preference pane’s bundle.

var mainNibName: String

The name of the preference pane’s nib file.

var mainView: NSView

The main view of the preference pane.

### Selecting and Deselecting the Preference Pane

func willSelect()

Notifies the preference pane that the main app is about to display the preference pane’s main view.

func didSelect()

Notifies the preference pane that the main app has just displayed the preference pane’s main view.

func willUnselect()

Notifies the preference pane that the main app is about to stop displaying the preference pane’s main view.

func didUnselect()

Notifies the preference pane that the main app has just stopped displaying the preference pane’s main view.

var isSelected: Bool

A Boolean value that indicates whether the preference pane is currently selected.

var shouldUnselect: NSPreferencePaneUnselectReply

A Boolean value that indicates whether the preference pane is able to be deselected.

enum NSPreferencePaneUnselectReply

Constants that indicate the preference pane’s availability to be deselected.

func reply(toShouldUnselect: Bool)

Notifies the main application of the preference pane’s ability to be deselected.

### Handling keyboard focus

var firstKeyView: NSView?

The first view in the keyboard focus chain.

var initialKeyView: NSView?

The view that should have keyboard focus when the pane is selected.

var lastKeyView: NSView?

The last view in the keyboard focus chain.

var autoSaveTextFields: Bool

A Boolean value that indicates whether text fields save their values before changing preference panes.

### Help Menu support

func updateHelpMenu(with: [[String : String]]?)

Updates the help menu.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

