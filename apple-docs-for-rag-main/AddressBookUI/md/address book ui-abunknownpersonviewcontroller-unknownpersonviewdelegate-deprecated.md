

- Address Book UI
- ABUnknownPersonViewController
-  unknownPersonViewDelegate Deprecated

Instance Property

# unknownPersonViewDelegate

The unknown-person view controller delegate.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
unowned(unsafe) var unknownPersonViewDelegate: (any ABUnknownPersonViewControllerDelegate)? { get set }
```

Deprecated

Use +\[CNContactViewController viewControllerForUnknownContact:\] from ContactsUI.framework instead

## Discussion

The delegate must adopt the ABUnknownPersonViewControllerDelegate protocol.

## See Also

### Responding to View Controller Interactions

protocol ABUnknownPersonViewControllerDelegate

The methods you use to respond to events in an unknown person view controller.

Deprecated

