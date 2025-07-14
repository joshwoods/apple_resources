

- Preference Panes
- NSPreferencePane
-  mainViewDidLoad() 

Instance Method

# mainViewDidLoad()

Notifies the preference pane that the main view is set up and prepared to be displayed.

Mac Catalyst 14.0+macOS 10.1+

``` source
func mainViewDidLoad()
```

## Discussion

Invoked by the default implementation of loadMainView() after the main nib file has been loaded and the main view of the preference pane has been set. The default implementation does nothing. Override this method to initialize the main view with the current preference settings.

## See Also

### Loading the Main View

func loadMainView() -> NSView

Loads the preference pane’s user interface into its main view.

func assignMainView()

Locates and assigns the preference pane’s main view from the nib file loaded by loadMainView().

