

- Preference Panes
- NSPreferencePane
-  reply(toShouldUnselect:) 

Instance Method

# reply(toShouldUnselect:)

Notifies the main application of the preference pane’s ability to be deselected.

Mac Catalyst 14.0+macOS 10.1+

``` source
func reply(toShouldUnselect shouldUnselect: Bool)
```

## Discussion

If you override shouldUnselect to return NSPreferencePaneUnselectReply.unselectLater, you must invoke reply(toShouldUnselect:) when you have determined whether or not the preference pane can be deselected.

You should not override this method.

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

var shouldUnselect: NSPreferencePaneUnselectReply

A Boolean value that indicates whether the preference pane is able to be deselected.

enum NSPreferencePaneUnselectReply

Constants that indicate the preference pane’s availability to be deselected.

