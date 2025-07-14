

- Preference Panes
- NSPreferencePane
-  assignMainView() 

Instance Method

# assignMainView()

Locates and assigns the preference pane’s main view from the nib file loaded by loadMainView().

Mac Catalyst 14.0+macOS 10.1+

``` source
func assignMainView()
```

## Discussion

The default implementation sets the receiver’s main view to the content view of the window referenced by the `_window` outlet. Before returning, assignMainView() releases the window and sets the `_window` outlet to `nil`. Returns the main view if successful, `nil` otherwise.

Override this method if your main view is located in the nib file loaded by loadMainView(), but is not the content view of a window in the file. Call NSPreferencePane to set the main view of the preference pane before returning. Also call NSPreferencePane, NSPreferencePane, and NSPreferencePane to set the initial, first, and last keyboard focus views, respectively.

## See Also

### Loading the Main View

func loadMainView() -> NSView

Loads the preference pane’s user interface into its main view.

func mainViewDidLoad()

Notifies the preference pane that the main view is set up and prepared to be displayed.

