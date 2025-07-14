

- UIKit
- UIDocumentMenuViewController
-  delegate Deprecated

Instance Property

# delegate

The document menu’s delegate.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
weak var delegate: (any UIDocumentMenuDelegate)? { get set }
```

## Discussion

The delegate must adopt the UIDocumentMenuDelegate protocol.

## See Also

### Getting the user-selected document picker

protocol UIDocumentMenuDelegate

A set of methods that you must implement to track user interactions with a document menu view controller.

Deprecated

