

- AppKit
- NSWindow
-  tabbingIdentifier 

Instance Property

# tabbingIdentifier

A value that allows a group of related windows.

macOS 10.12+

``` source
@MainActor
var tabbingIdentifier: NSWindow.TabbingIdentifier { get set }
```

## Discussion

By default, a window generates a tabbing identifier from inherent window properties, such as the window class name, the delegate class name, the window controller class name, and some additional state. Group windows together by using the same tabbing identifier.

## See Also

### Managing Window Tabs

class var allowsAutomaticWindowTabbing: Bool

A Boolean value that indicates whether the app can automatically organize windows into tabs.

class var userTabbingPreference: NSWindow.UserTabbingPreference

A value that indicates the user’s preference for window tabbing.

var tab: NSWindowTab

An object that represents information about a window when it displays as a tab.

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

