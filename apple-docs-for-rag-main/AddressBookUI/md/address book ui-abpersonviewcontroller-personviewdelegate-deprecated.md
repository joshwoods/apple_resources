

- Address Book UI
- ABPersonViewController
-  personViewDelegate Deprecated

Instance Property

# personViewDelegate

The person-view controller delegate.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
unowned(unsafe) var personViewDelegate: (any ABPersonViewControllerDelegate)? { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

The delegate must adopt the ABPersonViewControllerDelegate protocol.

## See Also

### Responding to View Controller Interactions

protocol ABPersonViewControllerDelegate

The `ABPersonViewControllerDelegate` protocol declares the interface that must be implemented by ABPersonViewController delegates.

Deprecated

