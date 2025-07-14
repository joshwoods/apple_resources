

- Preference Panes
- NSPreferencePane
-  loadMainView() 

Instance Method

# loadMainView()

Loads the preference pane’s user interface into its main view.

Mac Catalyst 14.0+macOS 10.1+

``` source
func loadMainView() -> NSView
```

## Discussion

The default implementation loads the main nib file (identified by mainNibName) and calls assignMainView() to set the main view of the preference pane. Returns the main view if successful, or `nil` otherwise.

Subclasses should rarely need to override this method. Override this method if you need to use a non-nib based technique for creating the main view. Call NSPreferencePane to set the main view of the preference pane before returning. Also call NSPreferencePane, NSPreferencePane, and NSPreferencePane to set the initial, first, and last keyboard focus views, respectively.

## See Also

### Loading the Main View

func assignMainView()

Locates and assigns the preference pane’s main view from the nib file loaded by loadMainView().

func mainViewDidLoad()

Notifies the preference pane that the main view is set up and prepared to be displayed.

