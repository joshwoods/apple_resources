

- Objective-C Runtime
- NSObject
-  chooseIdentityPanelShowHelp(\_:) 

Instance Method

# chooseIdentityPanelShowHelp(\_:)

Implements custom help behavior for the modal panel.

macOS 10.4+

``` source
func chooseIdentityPanelShowHelp(_ sender: SFChooseIdentityPanel!) -> Bool
```

## Parameters 

`sender`  

The choose identity panel for which to implement custom help.

## Discussion

You can use this delegate method to implement custom help if you call the setShowsHelp(_:) method to display a help button in the sheet or panel. If you are not implementing custom help, do not implement this method.

## See Also

### Related Documentation

@MainActor func setShowsHelp(_ showsHelp: Bool)

Displays a Help button in the sheet or panel.

@MainActor weak var delegate: (any NSWindowDelegate)? { get set }

The window’s delegate.

