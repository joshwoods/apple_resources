

- StoreKit
- SKRequest
-  delegate Deprecated

Instance Property

# delegate

The delegate of the request object.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
weak var delegate: (any SKRequestDelegate)? { get set }
```

Deprecated

No longer supported

## Discussion

The delegate must adopt the SKRequestDelegate protocol, although most subclasses of SKRequest provide a more specific protocol to implement.

## See Also

### Accessing the Delegate

protocol SKRequestDelegate

Common methods that are implemented by delegates for any subclass of the `SKRequest` abstract class.

Deprecated

