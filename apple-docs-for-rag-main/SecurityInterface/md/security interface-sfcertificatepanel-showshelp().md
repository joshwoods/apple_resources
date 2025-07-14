

- Security Interface
- SFCertificatePanel
-  showsHelp() 

Instance Method

# showsHelp()

Indicates whether the help button is currently set to be displayed.

macOS 10.4+

``` source
@MainActor
func showsHelp() -> Bool
```

## Discussion

This method returns true if the help button is currently set to be displayed.

## See Also

### Providing Help

func setHelpAnchor(String!)

Sets the help anchor string for the sheet or modal panel.

func setShowsHelp(Bool)

Displays a Help button in the sheet or panel.

func helpAnchor() -> String!

Returns the current help anchor string for the sheet or panel.

