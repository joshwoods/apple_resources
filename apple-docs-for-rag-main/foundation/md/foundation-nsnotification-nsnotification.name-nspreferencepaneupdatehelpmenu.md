

- Foundation
- NSNotification
- NSNotification.Name
-  NSPreferencePaneUpdateHelpMenu 

Type Property

# NSPreferencePaneUpdateHelpMenu

Notifies observers that your help menu content changed.

macOS 10.0+

``` source
static let NSPreferencePaneUpdateHelpMenu: NSNotification.Name
```

## Discussion

The object of the notification is an array of dictionaries containing the new help menu contents.

## See Also

### PreferencePanes

static let NSPreferencePaneCancelUnselect: NSNotification.Name

Notifies observers that the preference pane should not be deselected.

static let NSPreferencePaneDoUnselect: NSNotification.Name

Notifies observers that the preference pane may be deselected.

static let NSPreferencePaneSwitchToPane: NSNotification.Name

Notifies observers that the user selected a new preference pane.

static let NSPreferencePrefPaneIsAvailable: NSNotification.Name

Notifies observers that the system preferences app is available to display your preferences.

