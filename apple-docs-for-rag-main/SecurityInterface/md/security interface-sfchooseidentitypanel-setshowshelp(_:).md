

- Security Interface
- SFChooseIdentityPanel
-  setShowsHelp(\_:) 

Instance Method

# setShowsHelp(\_:)

Displays a Help button in the sheet or panel.

macOS 10.4+

``` source
@MainActor
func setShowsHelp(_ showsHelp: Bool)
```

## Parameters 

`showsHelp`  

Set to true to display the help button. The help button is hidden by default.

## Discussion

When a user clicks the help button, the choose identity panel first checks the delegate for a certificatePanelShowHelp(_:) method. If the delegate does not implement such a method, or the delegate method returns false, then the NSHelpManager method openHelpAnchor(_:inBook:) is called with a `nil` book and the anchor specified by the setHelpAnchor(_:) method. An exception is raised if the delegate returns false and there is no help anchor set.

## Topics

### Related Documentation

func chooseIdentityPanelShowHelp(_ sender: SFChooseIdentityPanel!) -> Bool

Implements custom help behavior for the modal panel.

@MainActor func openHelpAnchor(_ anchor: NSHelpManager.AnchorName, inBook book: NSHelpManager.BookName?)

Finds and displays the text at the given anchor location in the given book.

func showsHelp() -> Bool

Indicates whether the help button is currently set to be displayed.

## See Also

### Providing Help

func setHelpAnchor(String!)

Sets the help anchor string for the sheet or modal panel.

func helpAnchor() -> String!

Returns the current help anchor string for the sheet or panel.

func showsHelp() -> Bool

Indicates whether the help button is currently set to be displayed.

