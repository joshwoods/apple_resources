

- Preference Panes
- NSPreferencePane
-  isSelected 

Instance Property

# isSelected

A Boolean value that indicates whether the preference pane is currently selected.

Mac Catalyst 14.0+macOS 10.1+

``` source
var isSelected: Bool { get }
```

## Discussion

true if preference pane is currently selected by user, false otherwise.

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

var shouldUnselect: NSPreferencePaneUnselectReply

A Boolean value that indicates whether the preference pane is able to be deselected.

enum NSPreferencePaneUnselectReply

Constants that indicate the preference pane’s availability to be deselected.

func reply(toShouldUnselect: Bool)

Notifies the main application of the preference pane’s ability to be deselected.

