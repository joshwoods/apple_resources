

- Preference Panes
- NSPreferencePane
-  shouldUnselect 

Instance Property

# shouldUnselect

A Boolean value that indicates whether the preference pane is able to be deselected.

Mac Catalyst 14.0+macOS 10.1+

``` source
var shouldUnselect: NSPreferencePaneUnselectReply { get }
```

## Discussion

The possible values are described in Help Menu Support. The default implementation always returns NSPreferencePaneUnselectReply.unselectNow. Override this method if your pane needs to cancel or delay a deselect action. If you override this method to return NSPreferencePaneUnselectReply.unselectLater, you must invoke reply(toShouldUnselect:) when you have determined whether or not the deselection can occur.

## See Also

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

enum NSPreferencePaneUnselectReply

Constants that indicate the preference pane’s availability to be deselected.

func reply(toShouldUnselect: Bool)

Notifies the main application of the preference pane’s ability to be deselected.

