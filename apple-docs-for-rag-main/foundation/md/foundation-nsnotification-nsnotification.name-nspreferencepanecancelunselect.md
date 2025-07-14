

- Foundation
- NSNotification
- NSNotification.Name
-  NSPreferencePaneCancelUnselect 

Type Property

# NSPreferencePaneCancelUnselect

Notifies observers that the preference pane should not be deselected.

macOS 10.0+

``` source
static let NSPreferencePaneCancelUnselect: NSNotification.Name
```

## Discussion

Posted when reply(toShouldUnselect:) is invoked with an argument of false after shouldUnselect has returned a value of NSPreferencePaneUnselectReply.unselectLater.

## See Also

### PreferencePanes

static let NSPreferencePaneDoUnselect: NSNotification.Name

Notifies observers that the preference pane may be deselected.

static let NSPreferencePaneSwitchToPane: NSNotification.Name

Notifies observers that the user selected a new preference pane.

static let NSPreferencePaneUpdateHelpMenu: NSNotification.Name

Notifies observers that your help menu content changed.

static let NSPreferencePrefPaneIsAvailable: NSNotification.Name

Notifies observers that the system preferences app is available to display your preferences.

