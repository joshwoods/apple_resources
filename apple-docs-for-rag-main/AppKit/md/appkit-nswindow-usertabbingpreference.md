

- AppKit
- NSWindow
-  userTabbingPreference 

Type Property

# userTabbingPreference

A value that indicates the user’s preference for window tabbing.

macOS 10.12+

``` source
@MainActor
class var userTabbingPreference: NSWindow.UserTabbingPreference { get }
```

## Discussion

This value indicates the user’s preference for window tabbing as set in System Preferences. Check this preference any time you create a new window. For a list of possible values, see NSWindow.UserTabbingPreference.

## See Also

### Managing Window Tabs

class var allowsAutomaticWindowTabbing: Bool

A Boolean value that indicates whether the app can automatically organize windows into tabs.

var tab: NSWindowTab

An object that represents information about a window when it displays as a tab.

var tabbingIdentifier: NSWindow.TabbingIdentifier

A value that allows a group of related windows.

typealias TabbingIdentifier

A value that allows a group of related windows.

func addTabbedWindow(NSWindow, ordered: NSWindow.OrderingMode)

Adds the provided window as a new tab in a tabbed window using the specified ordering instruction.

var tabbingMode: NSWindow.TabbingMode

A value that indicates when a window displays tabs.

var tabbedWindows: [NSWindow]?

An array of windows that display as tabs.

func mergeAllWindows(Any?)

Merges all open windows into a single tabbed window.

func selectNextTab(Any?)

Selects the next tab in the tab group in the trailing direction.

func selectPreviousTab(Any?)

Selects the previous tab in the tab group in the leading direction.

func moveTabToNewWindow(Any?)

Moves the tab to a new containing window.

func toggleTabBar(Any?)

Shows or hides the tab bar.

func toggleTabOverview(Any?)

Shows or hides the tab overview.

var tabGroup: NSWindowTabGroup?

A group of windows that display together as a tab group.

