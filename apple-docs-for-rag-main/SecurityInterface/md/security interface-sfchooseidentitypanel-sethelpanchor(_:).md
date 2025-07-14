

- Security Interface
- SFChooseIdentityPanel
-  setHelpAnchor(\_:) 

Instance Method

# setHelpAnchor(\_:)

Sets the help anchor string for the sheet or modal panel.

macOS 10.4+

``` source
@MainActor
func setHelpAnchor(_ anchor: String!)
```

## Parameters 

`anchor`  

The new help anchor string.

## Discussion

You may call this function to set a help anchor string if you display a help button in the sheet or modal panel and do not implement the delegate method certificatePanelShowHelp(_:), or if the delegate method returns false. If you display a help button, do not set a help anchor string, and do not implement a delegate, the certificate panel displays a default help page (“What is a digital identity?”).

## Topics

### Related Documentation

func chooseIdentityPanelShowHelp(_ sender: SFChooseIdentityPanel!) -> Bool

Implements custom help behavior for the modal panel.

func setShowsHelp(Bool)

Displays a Help button in the sheet or panel.

func helpAnchor() -> String!

Returns the current help anchor string for the sheet or panel.

## See Also

### Providing Help

func setShowsHelp(Bool)

Displays a Help button in the sheet or panel.

func helpAnchor() -> String!

Returns the current help anchor string for the sheet or panel.

func showsHelp() -> Bool

Indicates whether the help button is currently set to be displayed.

