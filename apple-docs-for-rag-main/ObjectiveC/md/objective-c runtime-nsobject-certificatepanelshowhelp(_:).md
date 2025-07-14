

- Objective-C Runtime
- NSObject
-  certificatePanelShowHelp(\_:) 

Instance Method

# certificatePanelShowHelp(\_:)

Implements custom help behavior for the modal panel.

macOS 10.4+

``` source
func certificatePanelShowHelp(_ sender: SFCertificatePanel!) -> Bool
```

## Parameters 

`sender`  

The certificate panel for which to implement custom help.

## Discussion

You can use this delegate method to implement custom help if you call the setShowsHelp(_:) method to display a help button in the sheet or panel. If you are not implementing custom help, do not implement this method.

## See Also

### Related Documentation

@MainActor weak var delegate: (any NSWindowDelegate)? { get set }

The window’s delegate.

@MainActor func setShowsHelp(_ showsHelp: Bool)

Displays a Help button in the sheet or panel.

